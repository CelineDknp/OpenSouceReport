# Report : open source strategy project (contribution to an existing open source project)

## Useful informations
Author : Céline DEKNOP
Noma : 4106144
Project : [Oppia](https://github.com/oppia/oppia)

## Phase 1 : Looking for a project

Having no real itch to fix something in any software or app I was using, it took me some time to find an idea.

My first one was to see if I could contribute in a community I'm already a part of : devRant, which is a "rant site" intended only for developers. I put a post up asking for opinion, and discovered in the process that the project was *not* open source, which is quite funny.

I still got council from the community, who pointed me towards a compilation of good projects to start with. I browsed them, to find out that most of them where using technologies that I didn't know; which was honestly more work that what I was intending to put into it.

I then found Oppia, which I won't use, but I think is meaningful : it aims at helping students that have no real education get one for themselves. It also seems to be quite organised and to have a lot of contributors, since there is a Google Form to fill out answering questions about your background in programming and what you want to do to help the community. Based on that, they send you an e-mail pointing to an issue to start with.

I waited for a bit, but it was late at night, so I saw the response on the next day : I was assigned backend test for files missing them. It is not my favorite task to write tests, but I could definitely use some practice. I also have someone to contact on their gitter chat. Off to contribute I go !

### Phase 1.5 : the procrastination
Since I'm "early", I spend the next 5 weeks saying that I should get to starting my contribution, always finding excuses not to. It was -at least to me- quite expected since the project spans over the whole half year.

## Phase 2 : discovering the project
After receiving a mail from someone in the Oppia team asking me if I needed help to start contributing, I started to feel guilty, and actually sat down to look at the project.

I followed all the instructions to fork, and dived into the documentation, which is luckily well-written and seems to be not too outdated. The codebase is huge, which makes it quite hard to grasp, but I keep going under the motivation of the [gitter chat](https://gitter.im/oppia/oppia-chat).

After a good hour of opening random files to find the one that I'm going to write test for, I finally settle for one I understand enough and get to it : *core/storage/email/gae_models.py*, I choose you !

## Phase 3 : actually writing code
Oppia has a nice tool to show you the test coverage, with percentages and lines that are not tested (I had problems running it at first, but the chat fixed them), so it's quite easy to see what tests are missing, and since most of them are already started, you have something to base your code of. I see why those issues are newbie-friendly.

After some time writing and seeing the coverage go up (from 75 to 82), I run into what I consider being a bug, or at least a problem : one function is not returning what it says it is on the `@returns`. I head to the gitter chat to report the problem and ask for what to do, so I have to interrupt and wait for an answer.
 
The next day, I have an answer, and it seems like I have uncovered a bug ! I'm asked to make a peer request out of it :
![screen of the gitter chat](PR.png "Gitter chat answer")

I ask details on how to do it correctly and go back to test-writing mode, until I get to 97% of test coverage. I don't really know how to go up to 100% and would like to ask for advices, but I'm still waiting on some responses on the gitter chat, so I decide to wait and stop for the day.

## Phase 4 : switching advice strategy
After two weeks without answer from the chat, I decide to send an e-mail instead, asking for help in the testing process and details about the pull request. I get an answer in a few days and get back to work.

First, I'm told to just do a pull request without reporting the bug, since it's so small. I wrap my corrections and work for a while on the push, since they have a very specific linter, as well as Travis tests that need to pass. When I get the all clear, I open [my first pull request](https://github.com/oppia/oppia/pull/5928) to the project ! I quickly fix a few things with the help of a contributor, and get my first green flag for the PR. Only thing left to do is to wait for it to be merged.

I then go back to the testing, since I'm 90% of the way done, it would be stupid to not finish them. With the helpful advices of my correspondant, I get to the point where I'm satisfied with the tests and don't know how to acheive a higher coverage.

After a lot of fighting with the linter and way too much commits, I'm done with my tests and start my [second pull request](https://github.com/oppia/oppia/pull/5959).

By that time, the first pull request have been accepted, but the second one have not (so far). It is also time to turn in this report, but I'd expect to have the second one merged for the oral exam.

## Conclusion
I think I acheived the goal of the project which was to take part in an Open-Souce project not belonging to UCL. The community was very welcoming and active, which made my experience quite nice.

Following your instructions, I also would like to apologise for the not very formal tone of this report, if you feel like I should. I took you seriously when you told us to apologise rather than ask, so I did it this the way I would actually write a journal. It was way more fun for me to do it like that, and I think it is also more entertaining to read.