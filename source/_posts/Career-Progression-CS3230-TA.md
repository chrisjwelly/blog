---
title: 'Career Progression: CS3230 TA'
date: 2022-01-03 21:10:21
tags:
---

<!--toc-->
## Introduction and Motivation
Around 1.5 years ago, when I was [teaching CS2040S](https://chrisjwelly.github.io/blog/2020/08/08/The-CS2040S-teaching-experience/), I once joked with my students that since I taught CS1101S and CS2040S, a natural career progression would be to teach CS3230 next. I truly meant it as a joke, but little did I know back then that I would eventually go on to do it.

[CS3230 Design and Analysis of Algorithms](https://nusmods.com/modules/CS3230/design-and-analysis-of-algorithms) was taught by Prof Arnab Bhattacharrya in the recent semester (AY21/22 Sem 1). The module is part of the graduation requirements for computer science majors, and I believe computer engineering majors have the option to take this module to fulfill their requirements. It builds on CS2040S, providing more advanced tools and techniques to design (divide & conquer, greedy, dynamic programming) and analyse (amortisation, randomised analysis) algorithms. Theoretical content such as the famous "P vs NP" problem is also briefly touched upon.

I was initially not even thinking of teaching the module. How it came to be was that my previous CS3230 tutor was offered by Prof Arnab to teach, but he could not due to his commitments. My tutor then asked if I would be willing to teach in his place. I happened to have sat in Prof Arnab’s other classes before, and felt like I could be confident in the quality of his teaching (which was a complaint for other instructors in previous semesters). Moreover, I also have gained confidence in my own abilities over the semesters. Lack of confidence was one of the reasons I had not taken it up sooner. The final reason was because in the same semester, I was going to take CS5234 Algorithms at Scale. I thought CS3230 would be a good way for me to revise my fundamentals as well. A little fun fact is that when I taught CS1101S, I took CS2040S. When I taught CS2040S, I took CS3230. Then when I taught CS3230, I took CS5234. It's almost as if I taught things in order to solidify my fundamentals in the same semester. All things considered, I decided that it would be a good time and opportunity for me to take up the role.
<!--more-->

## The teaching experience
Compared to my previous experience teaching CS1101S and CS2040S, there are some notable differences this time. I have 18 students for the previous modules I taught combined. This time, I am teaching a total of 47 students. Moreover, I am teaching two 1-hour slots a week, rather than one 2-hour slot. This meant more students I am in-charge of, but less time to engage them. 

I opted not to do any grading. From my past experiences, grading is a huge time sink and quite a thankless job. So I did indicate in advance that I very much preferred to do teaching only, and I was fortunate to be granted that.

It should also be noted that this section is meant as my thoughts on my teaching experience, and it should not serve as a reflection of the difficulty of the module content.

### Preparation
Despite having an increased confidence in teaching the module, I still had concerns in whether I can do it well. During the break before the semester started, I took the opportunity to revise the module content. The primary material I visited was MIT’s own Design and Analysis of Algorithms course, [6.046J](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-046j-design-and-analysis-of-algorithms-spring-2015/), which is available on MIT OpenCourseWare. The material there is slightly more advanced and covers more than the NUS counterpart, so I only watched the relevant material. I was juggling all these with my summer internship, so I typically allocated 1.5 hours before my internship started, and another 1.5 hours at the end of the day. I used this time to watch the lecture and recitation videos, and I also attempted their assignment questions. I managed to consistently do this almost every day for 3-4 weeks, after which I unfortunately became less consistent. Though looking back again, I covered half of the 6.046J syllabus, which is nearly all of CS3230. So I suppose it was fine. It was good revision, and eventually I would occasionally link the relevant material at the end of my tutorials.

There were other supplementary materials as well. I perused the textbook [CLRS](https://en.wikipedia.org/wiki/Introduction_to_Algorithms) (which 6.046J uses too) before and throughout my teaching. I had hoped to attempt some of the exercises, but time is always an issue. I also found [Algorithm Design by Kleinberg and Tardos](https://www.cs.princeton.edu/~wayne/kleinberg-tardos/) to be a nifty resource, and it particularly helped me for the NP-completeness chapters. I personally found the NP-completeness chapter in CLRS to be more demanding than what CS3230 requires, so I sought out other resources and I think this textbook has the right amount of rigour.

### Teaching CS3230 with slides
As per the previous semesters, my teaching style revolves around the use of my own slides (it can be found [here](https://tinyurl.com/cs3230-ay2122s1-christian), but note that content differs across semesters). I elaborated on what’s on my mind when preparing slides in a [previous blog post](https://chrisjwelly.github.io/blog/2019/12/19/Reflections-on-being-a-CS1101S-Avenger/#1-1-Material-Preparation). But briefly, I prepare slides so that students can refer to it again in the future, and in order to allow me to be organised in my thoughts when teaching. Specific to CS3230, I didn’t quite like the slides that were officially distributed, so I sought to improve on it whenever I could.

However, unlike CS1101S and CS2040S, CS3230 tends to be more mathematical in nature. This is a new challenge for me in how to best deliver the content. Google Slides has almost zero support for mathematical content. Typesetting nicely is almost impossible. My clunky solution to this is to use LaTeX to produce the mathematical content that I need, or handwrite it on my iPad. I would then take screenshots and put it on my slides. One thing that I disliked in presentations involving maths is how people tend to put all the content in a single slide. I took care to add some animation and to explain step-by-step. I generally keep in mind that I am "presenting" the answers, rather than just "showing" them. If I did not take care to improve on the presentation, then I might as well just simply release the answers for students to read. 

{% asset_img answer-presentation.png "Step-by-step presentation" %}

Another thing I always take into consideration is how people either have short attention spans or simply do not remember what was discussed prior. This can be something as simple as forgetting what were the options to a multiple choice question. Whenever appropriate, I would always take snippets of relevant information from a previous slide and put it in one corner of the current slide. This might clutter the current slide and as such I handled it by putting such information in lighter colour, so that it doesn’t unnecessarily grab attention. The example below just shows the question statement posted in lighter colour.

{% asset_img relevant-info-lighter-colour.png "Showing some relevant information in lighter colour" %}

I also made an effort to be visual whenever I can, including the appropriate colour treatment. A slide with purely text can be very boring and unengaging. Whenever a visual illustration helps, I would take the effort to make it available. If not, I would also try to engage the audience with some memes. One of my proudest works is the illustration of a reduction from 3-SAT to Directed Hamiltonian Cycle. It is visually complicated which makes it difficult to be drawn by hand, so I think preparing it in my slides is worth the effort. 

{% asset_img dir-ham-cycle-reduction.png "Diagram to illustrate the reduction from 3-SAT to Directed Hamiltonian Cycle" %}

All these preparations took a lot of time. In some weeks, I stayed up to 4-5AM just to prepare them. I do estimate that I can spend from 6 to 10 hours a week just preparing slides. Almost all of my weeks have over 100 slides, with the most being up to max slides. I am personally very satisfied and proud with the work I have done preparing the slides. It may have been a lot of work, but I am preparing for at least 47 students; that is a huge responsibility. Later on in the semester, I have received several emails asking for access to my slides as well. It really makes me happy that people find it helpful!
{% asset_img slides-request.png "E-mail of a student not in my class requesting for slides" %}

### The online tutorial
Due to COVID-19, all the tutorials are online. It was my first time doing a fully-online teaching, so I was a little nervous too. As mentioned earlier, I taught 2 slots: one on Thursday, and one on Friday. While I do know some tutors prefer teaching back-to-back, I personally found it helpful not to. First of all, I could conduct a consultation session after each slot in order to give clarity when needed. Second of all, it gives me time to reflect and improve for the later slot. This was immensely useful since most of my slides are new. There were even occasions when students caught major typos in my slides, which I fixed for the next class. (I feel slightly bad for the earlier class though, my apologies!)

In the first class of the semester, I had asked people to turn on their cameras so I could at least see them. This was not sustainable, but it did not affect teaching so much. Still, I ended the semester not knowing how most of my students looked like. Once in school I joked with a friend that I could be walking past any of them without knowing, and an hour later I actually passed one of the students I happened to recognise. But I digress about tutorials.

Roughly how I conduct my tutorials is by giving a recap of the relevant topic for the tutorial, and then going through the assigned questions. The challenge here is that I only have a 1-hour slot, which means I should only spend around 50 minutes of contact time. I considered giving less of the recap, but I notice most students wouldn’t have done the tutorial anyway, and some people actually depended on my recaps. So I decided that it was worth the time. 

When going through the questions, we use this platform called Archipelago. Students can key in their answers into the platform. I personally view it as the primary form of engagement, which can give me signals whether people are understanding the content, or whether I should take more time to slow down and explain further. Giving students the time to think about the question might take away a lot of time for the tutorials, but I think it is helpful in the long run as students exercise their thinking a little bit more.

One thing I learned to be helpful was to stop frequently and to ask students to use the “thumbs-up” feature in Zoom. This really allowed me to gauge whether people understood what I just said or not. There were times when the signals hinted to me that I should repeat whatever I had just said.

I personally think the advantage of having online tutorials is being able to record the tutorials. I was initially afraid that it would mean less engagement in class, but to my pleasant surprise I still felt that the engagement was sufficient. Initially, I simply compiled all the recording links in one place that point to the Zoom recording. However, I received feedback about how the Zoom UI is rather suboptimal, so I eventually hosted them on YouTube as well. This is also helpful for future references, as I am unsure whether Zoom will be able to host the videos forever. For those interested, the playlist of my tutorials can be found [here](https://youtube.com/playlist?list=PL05ri2Yh409oa4OZmwLJze2O3IDHZyKFH).

Since tutorials are also online and I get less chance to interact with the students, one thing I tried to do to make class slightly more exciting is to play random videos before the start of the class. Here are a few samplers (no rickrolls, I promise): sample [one](https://www.youtube.com/watch?v=ih9zBLDr_ro), [two](https://www.youtube.com/watch?v=miomuSGoPzI) and [three](https://www.youtube.com/watch?v=V3uP7TtDeFc). I suppose I just didn’t want the wait before class starting to be awkward. Most of the time, no one said anything about it, except for that one time someone expected a funny video when I was playing a serious video for once. At the end of the semester, someone also commented that he would miss the random videos I play before class. That's nice.

A lot of things went relatively well, but much can be improved on. As for a personal reflection, I typically always either end on time, or overrun my classes. This is a consequence of having a detailed recap session, and attempting to go through the questions in more detail. Fortunately, the session is recorded so I could use it as a guarantee that students are not missing out. Punctuality is something I will try to work on in the future, and honestly I had expected this to be raised up in my teaching feedback. Surprisingly, no one raised it up. I am unsure as to what it might suggest -- are students okay with me overrunning it a bit? Or perhaps they simply do not mind?

### Miscellaneous materials
I also prepared some miscellaneous materials. One thing I did was to prepare a math prerequisite revision material. I understood that many of the students might have forgotten some of the discrete mathematics and algorithms that they learnt as a first-year undergraduate, so I decided to take the initiative to prepare the material accompanied by a video recording. I would think that the video was quite well-received. At the time of writing, it has 576 views and 37 likes. Pretty decent numbers, I think.

I also prepared additional material to go through content related to indicator random variables. It is a tool that is used to analyse randomised algorithms, and I notice that it can follow a rather fixed pattern. 

Initially, I meant to only share both of these materials to my tutorial groups, but upon mention of these materials to the teaching staff, Prof Arnab recommended that I release it for the cohort’s perusal. I’d like to think that it was worth doing so!

### Outside class
My personal fear when I was getting ready to manage 47 students was the interaction outside class. I was expecting a lot of private messages, and maybe requests for consultations as well. 

Personally it was not as bad as I imagined. I only met 1 or 2 students regularly for consultation outside my after-class hours. As for questions (via PMs) outside class, there were slightly more: perhaps around 5 people who regularly asked me questions? Not that bad. I also learnt to manage my own time and set boundaries better, so it was manageable in the end.

I initially attempted a policy where I will not answer questions 48 hours before the assignment deadline / exams. In the end, I could not bring myself to enforce it except for their midterm, since I also had quite a number of midterms to sit for. I’m still not sure how this policy is viewed by them, but I do think that they tend to forget its existence anyway. 

During recess and reading weeks, I took the effort to give additional consultation hours as I am sure they would have studied the material more closely and had questions. I ran one 1.5 hr session in recess week, and two 1.5 hr sessions in reading week. Attendance was decent, but I typically spend a considerable amount of time answering one question in detail. I wonder if some of the questions were left out as a consequence of this. 

Again, another nice thing about conducting all these online is that I could record them and timestamp some of the things I covered. At the very least, if someone else has the same question, I could save some time and redirect them to my video recording of consultations. I also took care to save the notes during consultation (I use Goodnotes on iPad), which they can refer to if needed.

## Conclusion
Overall, I enjoyed being a CS3230 TA this recent semester. I personally do think that CS3230 is not an easy module. It requires more-than-average mathematical maturity, and I do try my best to make the content as accessible as possible. I received some thank-you emails from people not even from my class and these are little things that motivate me to keep moving forward! Nothing makes me happier to hear that people are benefitting from the effort I put in to deliver the content.

{% asset_img thank-you-email.png "A thank-you email by a student" %}

Of course, I have to thank my own students as well! Thank you for patiently bearing with my teachings. I think I received pretty good feedback from them, but I will continue thinking of ways to improve! We took a class photo over zoom on our final tutorial! Funnily enough, it was the first time I saw some of them, hahaha

{% asset_img cs3230-tut07-ay2122s1.jpg "CS3230 AY21/22 S1 (Tut 07)" %}

{% asset_img cs3230-tut13-ay2122s1.jpg "CS3230 AY21/22 S1 (Tut 13)" %}

One more semester of university left, and I decided to teach CS3230 one more time! Hopefully, I get to do an even better job this coming semester!