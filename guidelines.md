# Haskell Study Group

## Guidelines

We will work through [_Haskell Programming from First Principles_](http://haskellbook.com/) (aka the "Haskell Book") by Christopher Allen and Julie Moronuki. The only prerequisites for participating are this book, a computer, and your person. An open mind is also recommended. No prior experience with Haskell, functional programming, or coding in general is required.

To prepare for your first visit, please do the following:

- **Join the [FPChat](http://fpchat-invite.herokuapp.com/) Slack community.**
All announcements pertaining to this study group will be sent out via Meetup and Slack. On the FPChat Slack, look for the `#haskell-study-group` channel.

- **[Purchase](https://gumroad.com/l/haskellbook) your own copy of the book (discount codes are available: see below).**
You will need your own copy on your own machine so you can work with the PDF and your terminal open side-by-side. This book was independently researched, written, and published by two Haskell developers working in their spare time to support education in functional programming. As a member of our strong and supportive community, we know you are too committed to the spirit of pure actions to "borrow" someone else's copy. They typeset it with LaTeX: give them a break!

- **Install [Stack](https://docs.haskellstack.org/en/stable/README/), the Haskell project development tool.**
If you are familiar with package managers like npm, pip, and apt, Stack is similar. You needn't show up already an expert, but do at least [learn the basics](resources/haskell-stack-notes.md). If you want to know everything, though, you could watch [this video](https://www.youtube.com/watch?v=sRonIB8ZStw). The most important thing: whatever you do, _do not install the Haskell Platform_.

- **Set up a project environment for your practice code, and familiarize yourself with GHC and GHCi.**
You don't need to do much more than create a directory for your code and make sure you know how to run the GHC compiler on your source files and GHCi when you need a REPL. I like to keep separate subdirectories for the individual chapters, but you can do whatever you find most convenient. Do not expect WiFi to be available at meeting locations, though every effort will be made to ensure its availability.

### Expectations

Participants in the study group will be expected to model and reinforce a culture of accountability. This entails everyone abiding by the norms of a supportive and rigorous classroom environment. Each week, you should complete the following tasks:

- Do all the reading.
- Type in all the code.
- Attempt all the exercises.
- Meet with a study partner to discuss your work.
- Attend the group meeting.

These expectations are not meant to make your life miserable but to provide a framework for your success. If you actually want to learn Haskell, consistency is the key—as with anything else. Since we'll be learning Haskell together in this group, it is essential that you work through each chapter on your own first so that you come to each group meeting prepared, knowing what you need help with and what you understand well enough to teach others. If you get stuck on a problem, keep moving, but do not just skip the exercises entirely.
#### For the sake of emphasis: _do not skip the exercises!_

If you are a complete beginner to programming or for whatever reason have trouble installing Haskell on your computer, don't worry about it! Come to the study group, and we'll help you figure it out. Fortunately, you don't even need a computer to work through Chapter 1—just pen, paper, and patience. So make sure you at least do that much, even if you require tech support.

**Discount codes** for the book are available if you genuinely need one. The authors do not want the price of the book to dissuade anyone from purchasing it, so please contact me if the cost is prohibitive, and you would like to request a discount. Please do not ask for a discount if you don't really need it. The number of codes I have is limited, and I want to reserve them for those who do.

### Conduct of code

By participating in this study group, you implicitly agree to conduct your coding as follows:

You will purchase your own copy of the Haskell Book. Anyone suspected of using an illegal copy will be removed from the group immediately.

Each week, prior to the group meeting, you will complete the assigned reading and attempt to complete the coding exercises to the best of your ability. If you do not make a genuine effort to complete your work, for whatever reason, you will not be permitted to join the group discussion that week. Participants who fail to complete their assignments twice in a row or three times total, or who are otherwise not making a good faith effort to keep up with the course schedule, may be asked to leave the group. If you find yourself struggling with the exercises, you should seek help at the meetings, from your study partner, or online.

You will make every effort to attend the weekly group meetings. Space is limited, so if you cannot commit to attending regularly, do not sign up. Participants who consistently miss meetings or RSVP without showing up will be removed from the group. If you cannot make it to a meeting, withdraw your RSVP as soon as possible.

In addition to the above, all study group participants are expected to make their best effort at being decent human beings. Participants whose behavior strays too far or too often beyond the reasonable boundaries of respect, kindness, and collegiality may be removed from the group at the discretion of the organizer.

The [Recurse Center](https://www.recurse.com) has a useful set of [social rules](https://www.recurse.com/manual#sub-sec-social-rules) that you should consider in effect for our meetings, too.

### Format

We will work through chapters 1–18 of the Haskell Book over the course of 12 weeks, meeting for about 2 hours each week. We may extend the meeting schedule to cover subsequent chapters if there is enthusiasm for doing so and the organizer is available.

**This is not a class**, however, so do not come expecting a lecture. Instead, you will have the opportunity to review your work and to discuss concepts and exercises that gave you difficulty when working through the book on your own.

You are encouraged to hew as closely to this regular, weekly schedule as you are able so as to maintain your momentum. That said, if life gets in the way, so be it: but do your best to catch up, and avoid skipping any material as each chapter builds on the last. We can always discuss exercises on Slack, but please refrain from posting your solutions publicly (including on GitHub).

### Signing up

All meetings will be announced on Meetup and Slack. You must RSVP to attend each meeting separately, as space is at a premium. If you cannot attend a meeting because it is full, please continue to work on your own, and come to a future meeting. Do not RSVP if you cannot attend. No-shows will not be allowed to attend subsequent meetings.

### Slides and other resources

See the [resources](resources) sub-directory in this repo for presentation slides, bonus exercises, and other materials used during study session meetings. If you have something pertinent to add, please submit a pull request.

### Schedule

**Week 1. Introduction. Lambda calculus.**
- Haskell Book, Chapter 1

**Week 2. Getting started with Haskell.**
- Chapters 2 and 3

**Week 3. Basic datatypes.**
- Review chapters 2 and 3
- Chapters 4 and 5

**Week 4. Types and Typeclasses.**
- Review chapters 4 and 5
- Chapter 6

**Week 5. Functional patterns. Working with recursion.**
- Review chapter 6
- Chapters 7 and 8

**Week 6. Lists and folding lists.**
- Review chapters 7 and 8
- Chapters 9 and 10

**Week 7. Algebraic datatypes.**
- Review chapters 9 and 10
- Chapters 11 and 12

**Week 8. Midpoint review. Testing with QuickCheck.**
- Review chapters 2-12
- Read and complete Chapter 13 on your own
- Chapter 14

**Week 9. Monoid and Semigroup.**
- Chapter 15

**Week 10. Functor.**
- Review Chapter 15
- Chapter 16

**Week 11. Applicative.**
- Review chapter 16
- Chapter 17

**Week 12. Monad. How to apply structure to your code. Conclusion.**
- Review chapter 17
- Chapter 18
- Read Chapter 19 on your own
- General review and look ahead

Meeting days, times, and locations may vary from week to week depending on the availability of space. If you can help with hosting future meetings, please contact me!

For details of specific meetings, see the Meetup page.

