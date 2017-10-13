# Cpp Con 2017 Notes

Notes, talk summaries, trip reports from Cpp Con 2017

published at: [Bartek's coding blog: Cpp Con 2017 Notes](http://www.bfilipek.com/2017/10/cpp-con-2017-notes.html)

## Intro

Links

* [Github with the slides and other materials](https://github.com/CppCon/CppCon2017)
* [YouTube channel](https://www.youtube.com/user/CppCon/videos)

## Trip Reports

* [Matt Godbolt’s CppCon 2017 Trip Report](https://xania.org/201710/cppcon-2017-trip-report)
* [Ben Deane's CppCon 2017 Trip Report](http://www.elbeno.com/blog/?p=1542)
* [Charles L. Wilcox's Trip Report](http://web.cynd.net/~willo/cppcon-2017-trip-report/)
* [Oliver Smith's Cpp Con 2017 Report](https://kfsone.wordpress.com/2017/10/01/cppcon-2017/)
* [Eva "Bunny" Conti: A Beginner's Guide to CPPCon 2017](https://bunnyladame.blogspot.no/2017/09/a-beginners-guide-to-cppcon-2017.html)
* [Viktor Kirilov - Cpp Con 2017 Trip report](http://onqtam.com/misc/2017-10-04-cppcon-2017-trip-report/)
* [Trip report: the JetBrains C++ team at CppCon 2017](https://blog.jetbrains.com/clion/2017/10/jb-cpp-at-cppcon-2017/)
* [Tim van Deurzen CppCon 2017 For Fun and Profit](http://blog.razzeal.org/posts/trip-report-cppcon-2017)
* [Quentin Duval - My CppCon 2017 Trip Report – 10 great talks to watch and learn from](https://deque.blog/2017/10/04/my-cppcon-2017-trip-report-10-great-talks-to-watch-and-learn-from)
* [Patrice Roy - À propos de cppcon 2017](http://h-deb.clg.qc.ca/Sujets/Orthogonal/cppcon2017.html ) _in french_
* [Isabella Muerte's CppCon 2017 Trip Report](https://izzys.casa/posts/cppcon-2017-trip-report.html)
* [Jens Weller - A CppCon 2017 trip report](https://www.meetingcpp.com/blog/items/A-CppCon-2017-trip-report.html)
* [Mathieu Ropert - CppCon 2017 trip report](https://mropert.github.io/2017/10/12/cppcon2017)


* IT Hare on Soft.ware reports: 
 * [#CPPCON2017 Day 0: IMO best posters](http://ithare.com/cppcon2017-day-0-imo-best-posters/)
 * [#CPPCON2017. Day 1. Hope to get something-better-than-chevron-hell](http://ithare.com/cppcon2017-day-1-hope-to-get-something-better-than-chevrone-hell/)
 * [#CPPCON2017. Day 2. Why Local Allocators are a Good Thing(tm) Performance-Wise, and Why I am Very Cautious about C++17 STL parallelized algos](http://ithare.com/cppcon2017-day-2-why-local-allocators-are-a-good-thing-and-why-i-am-very-cautious-about-stl-paralellized-algos/)
 * [#CPPCON2017. Day 3. The Future of C++](http://ithare.com/cppcon2017-day-3-the-future-of-c/)
 * [#CPPCON2017. Day 4. Async Rulezzz!](http://ithare.com/cppcon2017-day-4-async-rulezz/)
 * [CPPCON Day #5. Miscellaneous](http://ithare.com/cppcon-day-5-miscellaneous/)

## Talks

Here's a list of talks with a summary and they key points.

### Bjarne Stroustrup "Learning and Teaching Modern C++"

[CppCon 2017: Bjarne Stroustrup “Learning and Teaching Modern C++” - YouTube](https://www.youtube.com/watch?v=fX2W3nNjJIo)

* "We're all teachers" - this is a good talk, especially for all the people who teach other how to code: but not only bloggers, proffesors... but even for you when you advice/help your collegues from time to time.
* C++ was tought sometimes in a messy way, so we can do better.
* "if you write your own linked list (and use it in production code) you're cool". We cannot teach that way any more. It's just better to use STL.
* Simple example: Why range for loop is better than the old for loop (with i as the index).

### Matt Godbolt “What Has My Compiler Done for Me Lately? Unbolting the Compiler's Lid”

[CppCon 2017: Matt Godbolt “What Has My Compiler Done for Me Lately? Unbolting the Compiler's Lid”](https://www.youtube.com/watch?v=bSkpMdDe4g4)

[PDF slides](https://github.com/CppCon/CppCon2017/blob/master/Keynotes/What%20Has%20My%20Compiler%20Done%20for%20Me%20Lately%20-%20Unbolting%20the%20Compiler's%20Lid/What%20Has%20My%20Compiler%20Done%20for%20Me%20Lately%20-%20Unbolting%20the%20Compiler's%20Lid%20-%20Matt%20Godbolt%20-%20CppCon%202017.pdf)

* Matt's story: why he loves asm and how he started with Compiler Explorer.
* ASM 101, it's really not that hard to read some of the basic code. It might help you to understand your code better.
* Examples of how compilers might be smart. Math stuff mostly, but intresting to see how it's usually best to rely on the code generation.
* Tech stack behind Compiler Explorer

### Herb Sutter "Meta - Thoughts on Generative C++"

[PDF slides](https://github.com/CppCon/CppCon2017/blob/master/Keynotes/Meta%20-%20Thoughts%20on%20Generative%20C%2B%2B/Meta%20-%20Thoughts%20on%20Generative%20C%2B%2B%20-%20Herb%20Sutter%20-%20CppCon%202017.pdf)

[YouTube presentation](https://www.youtube.com/watch?v=4AfRAVcThyA&list=PLHTh1InhhwT6bwIpRk0ZbCA0N2p1taxd6&index=3)

At the beginning of the talk, Herb Sutter smartly “smuggled” very interesting concept of “Consistent comparison” in C++ which details you can find in proposal material [P0515 R0](http://open-std.org/JTC1/SC22/WG21/docs/papers/2017/p0515r0.pdf).

Main part was based on C++ static reflection – many links about this topic you can find on
[Jens Weller site](https://meetingcpp.com/blog/items/reflections-on-the-reflection-proposals.html). Herb shown how C++ can be easily extended using meta-classes that introduce another kind of abstraction. That was announcement of great changes that will come in near future.


### Carl Cook “When a Microsecond Is an Eternity: High Performance Trading Systems in C++”

[CppCon 2017: Carl Cook “When a Microsecond Is an Eternity: High Performance Trading Systems in C++”](https://www.youtube.com/watch?v=NH1Tta7purM)

[PDF slides](https://github.com/CppCon/CppCon2017/blob/master/Presentations/When%20a%20Microsecond%20Is%20an%20Eternity/When%20a%20Microsecond%20Is%20an%20Eternity%20-%20Carl%20Cook%20-%20CppCon%202017.pdf)

* High Frequency Trading in general earns money by buying and selling very often, and looking for small price changes. The success is to be faster than the competition.
 * Usually they have like 2.5us to react and do the trade... it's less time than a light travelling from top of BBurj Khalifa to the bottom!
* C++ is used because it's a relatively abstract language, gives zero cost overhead over the abstraction over the hardware.
 * They often have to check the generated code, so it's no coincidence that Compiler Explorer comes from that industry... check Matt's talk.
* Techniques covered (for the hot path, not for the whole code) 
 * removing branch prediction, using templates and compile time configuration (to avoid dynamic polimorphism, virtual method costs, eliminate branches) 
 * Lambdas are very expressive and still give a lot of power, they might be inlined.
 * Be carefull about memory allocations, use pool of pre allocated objects, delete on other thread
 * Carl advices to use exceptions (but not for the control flow!), they cost zero if they didn't throw.
 * Multithreading is usually avoided for low latency code, the hot path. They even disable all other cores and use just one.
 * Use data wisely, if you read something from the memory, use full cache lines
 * There's a comparision of various hash map approaches
 * in order to keep the cache hot, they might run simulations and only from time to time do the actual trade/response.
* As usually: measure measure measure :)
 * They setup a production system to measure it reliably
 
### Scott Wardle "EA's Secret Weapon - Packages and Modules"

[PDF slides](https://github.com/CppCon/CppCon2017/blob/master/Presentations/EA's%20Secret%20Weapon%20-%20Packages%20and%20Modules/EA's%20Secret%20Weapon%20-%20Packages%20and%20Modules%20-%20Scott%20Wardle%20-%20CppCon%202017.pdf)

[YouTube presentation](https://www.youtube.com/watch?v=NlyDUQS8OcQ)

* 15 years ago ElectronicArts faced the problem of code sharing and versioning. The company with many departaments around the world and code base running on multiple platforms decided to use code level, package approach. 
* A package is a C++ library source code conatining package name, package version, public includes (interface) and private includes and sources.
* Masterconfig file specifies list of all packages and versions ( including coinstraints ) on executable/project/team level.
* Each EA team build the packages on its own using configuration packages containing building flags.
* Packages are uploaded to package server, while source code is stored independently on VCS.
* Both packages and modules deals with public interfaces and hiding privates.

### Diego Rodriguez-Losada Gonzalez "Faster Delivery of Large C/C++ Projects with Conan Package Manager and Efficient Continuous Integration"

[YouTube presentation](https://www.youtube.com/watch?v=xA9yRX4Mdz0)

- Both inline functions ( declared in headers ) and archive ( static library ) functions used 
in shared library cause that the code is totally embedded into shared library. Any change the
code of static library or header function without rebuilding shared library cause code and behavioral divergence.

- [Conan.io](http://docs.conan.io/en/latest/) is a portable package manager that helps in dependencies management.
It provides package versioning, local binary cache, package server and integration with 
[JFrog](https://bintray.com/conan/conan-transit) - artifact repository. 

- [Conan.io](http://docs.conan.io/en/latest/) can be easily integrated with [Jenkins](https://jenkins.io) 
pipeline. Packages can be built, tested and uploaded to artifact repository using [Jenkinsfile ](https://jenkins.io/doc/book/pipeline/jenkinsfile/).

## Contributors

* (author) [Bartek from bfilipek.com](http://www.bfilipek.com)
* [Łukasz Rachwalski](https://github.com/lukaszrachwalski) - organizer of [C++ User Group Krakow](https://github.com/CppUserGroupCracow)
* [Yann Labou](https://github.com/yannlabou)
