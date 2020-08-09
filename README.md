# Christian's Blog
This repository contains Christian's blog powered by [Hexo](hexo.io), and using the [Tranquilpeak](https://github.com/LouisBarranqueiro/hexo-theme-tranquilpeak) theme.

## Setting-up
Requirements (see also [here](https://hexo.io/docs/#Requirements)):
* Node.js
* hexo-cli

This documentation is up-to-date as of Hexo 5.0. The Hexo version can be found in `package.json`.

Run the following commands in the terminal:
```bash
git clone --recurse-submodule https://github.com/chrisjwelly/blog.git
cd blog
npm install
cd themes/tranquilpeak
npm install && npm run prod
```

Note that in MacOS, there might be difficulties running `npm install` due to errors such as `Error: Cannot find module 'nan'`. If this occurs, run with `npm install --no-optional` instead.

To run the server, make sure you are in the root of the `blog` repository. Then, enter the following command in the terminal:
```bash
hexo server
```

If you have drafts in the blog and would like to show the drafts in the local server, run the following:
```bash
hexo server --draft
```

The server will be run in `http://localhost:4000/blog/`.

## Writing
The official documentation for writing can be found [here](https://hexo.io/docs/writing). 

Additionally, some features are specific to Tranquilpeak theme. Such features are labelled in this documentation. The full documentation can be found [here](https://github.com/LouisBarranqueiro/hexo-theme-tranquilpeak/blob/master/DOCUMENTATION.md).

### Creating and publishing
To create a new post:
```bash
hexo new <title>
```

To create a new draft:
```bash
hexo new draft <title>
```

To publish draft (turn it into a post):
```bash
hexo publish <title>
```

### Creating post excerpts (tranquilpeak):
Insert `<!--more-->` to define post excerpt. Whatever is above will still be displayed in the blog index page, but whatever below will be hidden and will only be shown if the blog post is visited.

### Displaying table of contents (tranquilpeak):
Display table of contents by using `<!--toc-->`

### Adding an image
To add an image:
1. Save the image in the corresponding folder with the same name as the blog post filename
2. Reference the image in the following manner: `{% asset_img [img_name] [title]%}

For example: `{% asset_img example.jpg "This is an example image" %}`
`[title]` will be shown when the mouse hovers over the picture.

Take note: Images do not seem to be rendered when the post is still a draft and the server is run with `hexo server --draft`. It seems that only upon publishing the draft as a post will the image appear.

## Deployment
The site is deployed to `https://chrisjwelly.github.io/blog/`. This is done automatically by Travis for every push to the `master` branch.

The configurations can be found in `.travis.yml`. Currently, it runs the script `travis.sh` to manually install the tranquilpeak theme before generating the website using the `hexo generate` command.
