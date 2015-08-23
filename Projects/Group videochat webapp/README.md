As the name suggests, the end goal of this project is to create a group videochat application. The time span is more than enough to explore, learn and create something quite functional. 

##Non-technical Guidelines
The workload is on the heavier side. Nevertheless, it is not necessary to compromise life outside OOP significantly to make a good application. 

1. Google your problem. The results are not always available in the first page and are heavily dependent on how you phrase your problem. If you are mindlessly going at it for more than 15 minutes and still don't have an answer, you might not be on the right track. Rephrase your search. There is a very good chance that someone else in this world has encountered the very same problem and has asked for help on a site like StackOverflow.

2. If you feel like you've wasted enough time searching for your problem (technical/non-technical), approach your project TA. They are, in most cases, sufficient to solve it. 

3. For serious problems (use your judgement), intimate the instructor of the course. 

4. As you go along, you'll find a difference of opinions among team members. Remember that each one of you have something to offer. Personally, if all it takes to have a better chance of reducing your workload is to listen to your team member's lazier idea, I'd take it up.

5. Stop complaining and divert that energy into debugging or asking someone for help. Having done the former last year, I can assure you that crafting ingenious paragraphs or neatly organized lists about the herculean nature of our problems is just a waste of time. (this document is a good example)

6. The internet can literally solve almost all your problems. Searching it is the most time-consuming part. Here is where the TAs come in. We have a fair idea of what can be done. We can help you with suggestions, not code. Use your resources effectively. You are expected to read and learn the pre-requisites like installing software, the programming language and other technology needed by yourself. The TAs can help you with it. The course is on Object Oriented Programming, __not Java__ or related technology.

##Technical Guidelines
1. The design stage is crucial in directing your development process. One simple and _acceptable_ assumption may reduce your workload significantly while preserving most of the functionality.

2. Reduce the number of use cases you have to a manageable 2 or 3 use cases. 

3. Here's where vague terms like _modularity_, _abstraction_ and so on help you. 
  1. __Abstraction__: Make conceptual blackboxes and describe things in simple English. This is the big picture. Ignore the gritty details of _how_ things will be done. Focus on _what_ needs to be done. If you have to figure out the answer to life itself at some point of time, make a box that says `Answer to life`. Worry about the how later.
  2. __Modularity__: Realize the abstractions into skeleton Java code (just the class names). Here is where you will make decisions about the hierarchy (`abstract`, `derived` classes and so on). 
  3. Feel free to look at more OOP buzzwords and interpret their relevance here :P

4. UML Diagrams are partly the materializations of your big-picture design decisions. While there are way too many arrows and decorative boxes, it is a standard and you have to abide by it. Look at Java projects and their corresponding UML diagrams (hint: use the [internet](https://www.google.co.in/search?q=example+uml+diagrams+java)) to get a simplistic idea. This is not a good enough substitute for the text. 

5. The other part of the UML diagram is a slightly detailed picture of _how_ things will work. Once again, it is not about the gritty details. Here is where you will partly worry about the how. If you have a box that reads `Play movie`, find a resource that will let you do it. 
  1. The resource should let you interface it with your project. In simple words, you should be able to use the Java library in your code without a lot of trouble. Some thing like `vlc.play("moviename.ext");`.
  2. The resource should be compatible/suitable to your requirements.
  3. There is always some library that suits your need. Scour the internet. You do __not__ have to reinvent the wheel.
  
6. Once the _what_ and _how_ are complete at the big-picture level, the UML diagram can give you a very clear way to go about coding.

(hopefully, this document will be periodically updated)
