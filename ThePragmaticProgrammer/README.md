# The Pragmatic Programmer

Notes by Syed Mohsin Bukhari

## Preface

**_Care about your craft (Tip 1)_**

**_Think! About your work (Tip 2)_**

## 1. Pragmatic Philosophy

### 1.1. It’s Your Life

* It’s your life, you own it, you run it, you create it

* "Why can’t you change it"

* **_You Have Agency (Tip 3)_**

* You can change your organization or change your organization

* If technology is passing by, make time to catch up (in your own time)

### 1.2. The Cat Ate My Source Code

* Take responsibility of the work assigned to you

* Think about your work and how to do it good

* Do not find excuses

* Think about your excuses and how they sound on the receiving end

* Do not blame your cat

* Have contingency plans

* Making contingency plans are your responsibility

* **_Provide options, do not make lame excuses (Tip 4)_**

* Team trust is important

### 1.3. Software Entropy

* Pay attention to small things

* Small things going wrong create chaos

* Keep your code pristine

* People have a tendency to keep clean things clean

* People have a tendency to ignore cleanliness when things are already not clean

* Do this even in case of emergencies (fires, deadlines, etc)

* **_Don’t live with broken windows (Tip 5)_**

### 1.4. Stone Soup and Boiled Frogs

Stone Soup

* Tell good things about your stone soup but make it well

* Improve your soup incrementally by adding ingredients one at a time

* Do not ask for all the ingredients at the same time

* Point out nice things that will result because of each ingredient

* People invest in on going success

* With limited resources, show people a glimpse of success and they will invest

* **_Be a catalyst for change (Tip 6)_**

Boiled Frogs

* **_Remember the big picture (Tip 7)_**

* Keep an eye out for minor changes

* Small things going wrong break the entire system

* Big changes are easy to spot but small changes are hard to spot

### 1.5. Good-Enough Software

* Software does not have to be perfect

* Good enough does not mean sloppy

* Good enough meets all requirements

* Transparent trade-offs between quality and time

* **_Make quality a requirements issue (Tip 8)_**

* Improve your software in multiple iterations

* Know when to stop

### 1.6. Your Knowledge Portfolio

* Knowledge assets diminish over time

* Invest in knowledge portfolio smartly:

  * Serious investors invest regularly—as a habit.

  * Diversification is the key to long-term success.

  * Balance between conservative and high-risk, high-reward investments.

  * Investors try to buy low and sell high for maximum return.

  * Portfolios should be reviewed and rebalanced periodically.

* **_Invest regularly in your knowledge portfolio (Tip 9)_**

* Technical investment tips

  * Learn at least one new language every year

  * Read a technical book each month

  * Read non-technical books too

  * Take classes

  * Participate in local user groups and meetups

  * Experiment with different environments (Windows/Linux, IDE/terminal)

  * Stay current

* Find answers to small questions you get asked that you don’t know the answer to

* **_Critically analyze what you read and hear (Tip 10)_**

* A few questions to ask while consulting

  * Ask the "Five Whys" (ask *why* at least five times, to dig deeper)

  * Who does this benefit? (*follow the money*)

  * What’s the context?

  * When and Where would this work? (think about future)

  * Why is this a problem?

### 1.7. Communicate

**_English is just another programming language (Tip 11)_**

* Know what you want to say

* Know your audience

* Choose your moment

* Choose a style

* Make it look good

* Involve your audience

* Be a listener

* Get back to people

  * **_It’s both what you say and the way you say it (Tip 12)_**

* Documentation

  * **_Build Documentation in, don’t bolt it on (Tip 13)_**

  * Put all documentation in code comments

  * Comment about design decisions etc. too

## 2. Pragmatic Approach

### 2.1. The Essence of Good Design

* There is a lot of "advice" floating around regarding *“Good Design”*

* **_Good design is easier to change than bad design (Tip 14)_**

* Easier To Change (ETC)

* Why is decoupling good? Because ETC

* Why is the single responsibility principle useful? Because ETC

* Why is naming important? Because ETC

* ETC is a value, not a rule

### 2.2. DRY - The Evils of Duplication

* Maintenance is an ever going process

* Every piece of knowledge must have a single, unambiguous, authoritative representation within a system

* **_DRY - Don’t Repeat Yourself (Tip 15)_**

* DRY is more important than code

* If you change one, you should not have to remember to change the other

* Types of duplication

  * Imposed duplication

  * Inadvertent duplication

  * Impatient duplication

  * Interdeveloper duplication

* Sources of duplication

  * Multiple representations of information (for e.g. different languages)

  * Documentation in code (for e.g. outdated docstrings in code)

  * Documentation and code (for e.g. code changes but documentation does not)

  * Language issues (for e.g. header and implementation separation)

  * Bad design (for e.g. unnormalized data, Point class contains x1, x2 AND length)

* Always develop uniform ways for accessing the services of a module

* Investment in avoiding duplication pays eventually even when deadlines are close

* Allow developers to communicate

* **_Make it easy to reuse (Tip 16)_**

* Not all repetition is knowledge duplication

  * Two function bodies can be same, for e.g.

    * validate_age(value)

      * validate_type(integer)

      * validate_min_integer(value, 0)

    * validate_quantity(value)

      * validate_type(integer)

      * validate_min_integer(value, 0)

### 2.3. Orthogonality

* Orthogonality helps with immediate improve in quality

* Helicopter controls are decidedly not orthogonal (that is why it is a very difficult job)

* **_Eliminate effects between unrelated things (Tip 17)_**

* When components are orthogonal, you can change one without worrying about the rest

* Gain productivity:

  * Simple orthogonal components are easy to design, code and unit test

  * Easiness in reuse

  * Reduction in effort due to reusability

* Reduce risk:

  * Easy to debug

  * Changes and fixes are localized to a particular area in code

  * Better tested code

  * Freedom to use any framework by any vendor

* Orthogonality applies to teams, work should be orthogonal, inter and intra team

* Systems should consist of sets of cooperative tools

* Don’t rely on the features of external software that you can’t control

* Techniques to maintain orthogonality:

  * Keep your code decoupled

  * Avoid global data

  * Avoid similar functions

* Be constantly critical of your code

* Use macros and style sheets for documentation appearance

* Think about the differences in the following with respect to orthogonality:

  * Multiple inheritance in C++

  * Implementation of multiple interfaces in Java

### 2.4. Reversibility

* Reversibility of decisions regarding architecture, vendors, frameworks is critical

* Tying to a certain kind of database in the beginning will not allow for change later

* Requirements, users and hardware change faster than we can change software

* Create abstractions around databases to treat them like persistence

* Databases are just an example, consider the cons of tying to a certain ML framework

* **_There are no final decisions (Tip 18)_**

* Reversibility in architecture, deployment and vendor integration should be considered

* Prepare for both scenarios, abstract out the fact whether the cat is dead or alive

* **_Forgo following fads (Tip 19)_**

### 2.5. Tracer Bullets

* Fix your direction through feedback, constantly check what is wrong and then adjust

* In dark knowing how to fire your bullets to hit the target exactly is a very difficult process

* Use dummy bullets after a few real bullets that ignite in the dark and help aim properly

* Tracer bullets operate in the same environment and constraints as the real bullets

* Tracer bullets get to target faster than calculated attack

* **_Use tracer bullets to find the target (Tip 20)_**

* Pros of tracer bullets:

  * Users get to see something working early

  * Developers build a structure to work in

  * You have an integration platform (helps to integrate new features very frequently)

  * You have something to demonstrate

  * You have a better feel for progress

* Tracer bullets don’t always hit their target

* Tracer bullets are not prototyping

  * Prototypes are disposable

  * Tracer code makes it in the final product

* Tracer code is based on the same framework as finished production code

### 2.6. Prototypes and Post-it Notes

* Prototypes cost less

* Prototypes target parts of the whole system

* Prototypes help analyze and expose risks

* Prototypes offer chances for correction at a greatly reduced cost

* Prototypes of cars are made of different material than the original car

* Prototypes for computational or performance aspects don’t necessarily need a GUI

* If you can’t give up on details while prototyping, go for tracer bullets instead

* Things to prototype:

  * Architecture

  * New functionality in an existing system

  * Structure or contents of external data

  * Third-party tools or components

  * Performance issues

  * User interface design

* Prototyping is a learning experience, its value lies in the lessons learned not in the code

* **_Prototype to learn (Tip 21)_**

* Prototypes can ignore:

  * Correctness (of data)

  * Completeness

  * Robustness

  * Style

* Prototyping architecture may not need code, it only needs to look into certain areas like:

  * Well defined responsibilities of major components

  * Collaborations between major components

  * Minimized coupling

  * Identification of potential sources of duplication

  * Acceptability of interface definitions and constraints

  * Every module has an access and path to the data it needs during execution

* When prototyping, make sure everyone knows that you are writing disposable code

* If you think your prototype will be misinterpreted as final code, use tracer bullets instead

### 2.7. Domain Languages

* Some languages are better at doing some things than other languages

* Make a mini-language for your users if they have a number of well bounded statements

* Your new language may not even execute, but only capture requirements

* End users don’t need to program in these languages

* It helps you work closer to client’s domain

* **_Program close to the problem domain (Tip 22)_**

* Each stakeholder might have different problem domains and hence different languages

* Mini-languages are line oriented and easily parsable

* You may extend an existing mini-language (e.g. Python)

* Data mini-languages

  * Describe a data structure (for e.g. Microsoft’s resource files)

  * Can compile to generate data objects for another language

* Imperative mini-languages

  * May contain control statements, control structures etc

  * May behave like normal languages but might not be object oriented

  * May only have sequential code execution

* Programmers don’t have to grovel around in C code

* Main application might not necessarily use the mini-language

### 2.8. Estimating

* Estimates help determine feasibility

* **_Estimate to avoid surprises (Tip 23)_**

* Estimates are relative

* Estimate of 6 months is better than 180 days because later implies more accuracy

* Estimate 125 working days as 6 months

* Choose the units of your answer to reflect the accuracy you want to convey

* Understand what is being asked when an estimate is required

* Build a model of the system and estimate roughly based on model

* Doubling the estimate might only give you a slight increase in accuracy

* Break the model into components and estimate for each component

* Give each parameter of each component a value

* Prioritize those parameters which are more impactful on the result

* Calculate the answers using parameter values

* Only in the simplest of cases will an estimate have a single answer

* If your estimate is wrong, do not discard, understand why it is wrong

* Keep track of your estimating prowess, see where you were wrong

* Iterate the schedule with the code

* WHAT TO SAY WHEN ASKED FOR AN ESTIMATE: You say "I will get back to you"

* You almost always get better estimates if you slow the process down

* Estimates given at the coffee machine will (like this coffee) come back to haunt you

* **_Iterate the schedule with code (Tip 24)_**

## 3. The Basic Tools

* Grow your set of tools with need

* The tools will become extensions of your hands

### 3.1. The Power of Plain Text

* As Pragmatic Programmers, our base material isn’t wood or iron, it’s knowledge

* Plain text is made up of printable characters in a form that can be understood directly

* XML and HTML are great examples of plain text

* **_Keep knowledge in plain text (Tip 25)_**

* Disadvantages of plain text

  * It may take more space to store than a compressed binary format

  * It may be computationally more expensive to interpret and process

* Even when your data needs to be stored differently, you keep metadata

* If there is a security risk then encrypt only that data, for e.g. MD5 hashes

* The Power of Text (Advantages)

  * Insurance against obsolescence

    * Human-readable data will outlive all other forms of data

    * You can parse plain text file with only partial knowledge of its format

  * Leverage

    * Virtually every tool in the computing universe can operate on text

    * Easy to use Source Code Control on plain text

  * Easier Testing

    * Easy to spot changes

* Lowest Common Denominator

  * You need to ensure that all parties can communicate using a common standard

  * Plain text is that standard

* In heterogeneous environments, the pros of plain text can outweigh all of the cons

### 3.2. Shell Games

* Shell (command line interface) is the centerpiece of your workshop

* Using shell you can automate your tasks

* A benefit of GUI is "What You See Is What You Get" (WYSIWYG)

* The disadvantage is "What You See Is **_All_** You Get" (WYSIAYG)

* GUI environments are normally limited to the capabilities that their designers intended

* Shell is faster at many tasks that combine functionality, for example:

  * Find all .c files modified more recently than your Makefile

  * Construct a zip/tar archive of my source

  * Which Java files have not been changed in the last week

  * Of those files, which use the **awt** libraries

* Combine shell commands into script files to automate things you do often

* **_Use the power of command shells (Tip 26)_**

* Play around with your command shell, invest some energy in becoming familiar with it

* It will make you more productive

* Read the GNU General Public Licence

* Windows CLI utilities are inferior to their UNIX counterparts, however, all is not lost

* Cygnus Solutions has a package, Cygwin with provides UNIX utilities in windows

* Some utilities don’t work as expected in Windows

### 3.3. Power Editing

* Editors, like tools are extension of your hand

* Use a single editor well

* **_Achieve editor fluency (Tip 27)_**

* The keys will sing as they slice their way through text and thought

* Make sure that the editor you choose is available on all platforms you use

* Editor features:

  * Configurable (e.g. keystroke bindings)

  * Extensible (to any new language)

  * Programmable (through macros or built-in scripting language)

* Other language specific features:

  * Syntax highlighting

  * Auto-completion

  * Auto-indentation

  * Initial code or document boilerplate

  * Tie-in to help systems

  * IDE-like features (compile, debug, and so on)

* It is meant to increase productivity

* When you create a new file using your editor it might include:

  * Name of the class or module filled in (derived from the filename)

  * You name and/or copyright statements

  * Skeletons for constructs in that language (constructor and destructor)

* Where to go from here:

  * I use only basic features of many different editors

    * Then pick a powerful editor and learn it well

  * I have a favorite editor, but I don’t use all of its features

    * Learn them, cut down the number of keystrokes you need to type

  * I have a favorite editor and use it where possible

    * Try to expand and use it for more tasks than you do already

  * I think you are nuts, Notepad is the best editor ever made

    * As long as you are happy and productive, go for it

    * But if you find yourself subject to "editor envy", then reevaluate

### 3.4. Version Control

* Reverting changes is essential

* You can always go back to a previous version of your software

* Version Control is far more than reverting changes

* It can help answer questions like:

  * Who made changes in this line of code

  * What’s the difference between the current version and last week

  * How many lines of code did we change in this release

  * Which files get changed most often

* It helps with bug-tracking, audit, performance and quality

* Branching allows multiple streams of code to be maintained in parallel

* Some systems allow two or more users to be working on the same set of files

* **_Always use version control (Tip 28)_**

* Keep everything in version control, including:

  * "Throw-away" prototypes

  * Documentation

  * Phone number lists

  * Memos to vendors

  * Makefiles

  * Build and release procedures

  * That little script that burns the CD master

  * Your editor configurations

  * The list of software installed

* It helps with builds that are *automatic *and *repeatable*

* Testing can be automated with every change

* But my team isn’t using source code control

  * Shame on them!

  * Sounds like an opportunity to do some evangelizing

  * Keep your code in source control and show its advantages to management

* Source Code Control is equally applicable to the things you do outside of work

* Keep configuration under source code control as well

### 3.5. Debugging

**Note**: _From this section onwards, I switched to the second edition of the book. I re-read the chapters/sections above from the second edition and made changes where necessary. However, from here on, there will be minor differences in formatting of notes to better suit the new edition._

* A moth caught in a relay in an early computer system, originated the term *computer bug*

#### Psychology of Debugging

* Debugging is a sensitive, emotional subject for many developers

* Instead of attacking it as a puzzle to solved

* You may encounter denial, finger pointing, lame excuses, or just plain apathy

* Embrace the fact that debugging is just *problem solving*

* **_Fix the problem, not the blame (Tip 29)_**

* It doesn't matter who was responsible for the bug

#### A Dugging Mindset

* Before debugging tune out all the project pressure due to deadlines

* Turn off many defenses that you use each day to protect your ego

* **_Don’t panic (Tip 30)_**

* It is very important to step back a pace and *think* about the symptoms

* If your reaction to a bug report is "that's impossible", you are plainly wrong

* Don't fix symptoms, fix the root cause and fix other problems along the way

#### Where to Start

* Start with a cleanly built (without warnings) code before finding a logical bug

* Set compiler warnings as high as possible to focus on harder problems at hand

* Gather all relevant data, and be accurate in data gathering

* Bug reporting is not an exact science

* Interview the user who reported the bug to gather more data

* Artificial tests don't exercise enough of an application

* Brutally test both boundary conditions and realistic end-user usage patterns

* You need to do this systematically (see [_Ruthless and Continuous Testing_](#ruthless-and-continuous-testing))

#### Debugging Strategies

* *Once you* think you know what is going on

  * It's time to find out what the program thinks is going on

  * Reproduce bugs

* Write test cases that isolate the bug, no need to follow 15 steps to reproduce it

* The act of writing test informs the solution

* **_Failing test before fixing code (Tip 31)_**

#### Coder in a Strange Land

* Many developers dive straight into code without reading the Exception message

* **_Read the damn error message (Tip 32)_**

* What if it is not a crash? What if it is just a bad result?

* Observe the variable values in the debugger as you move along

* Make sure you know how to move up and down the call stack

* Keep a paper and a pen to jot down where you started the bug chase

* To test senstivity to input values, feed data to a local deployment of app

  * Make sure it still crashes

  * [Binary chop](#the-binary-chop) the data until you isolate exactly which input values are problematic

* A previously working code crashed on you? Time for [binary chop](#the-binary-chop)!

#### The Binary Chop

* It's also sometimes called _Binary Search_

* For debugging, use the binary chop on _Stack Trace_ and/or datasets

* Revert to previously working releases using version control and compare stacks

* _Tracing statements_ are little messages like `I am here` and `value of x=2`

* _Tracing statements_ should be in a regular, consistent format for automatic parsing

  * To track down resource leaks, you can count the number of `open` and `close` commands

* Explain your problems to a rubber duck, to get a solution

  * While explaining, you might find the solution yourself

* Always assume first that the 3rd party libarary/OS is not broken even if it is

* A senior developer was convinced that `select` is broken, however, it wasn't

* **_"select" isn’t broken (Tip 33)_**

* If you made a little change and the app crashed, it is probably that little change

* If you are surprised by a bug, re-evaluate your truths

* The amount of surprise is directly proportional to the amount of trust and faith

* **_Don’t assume it - Prove it (Tip 34)_**

* Whatever happened, make sure you know if it happens again

* If it took a long time to find the bug, find out why and fix this

  * Use better testing hooks

  * Write a log file analyzer

* If bug arose due to one person's wrong assumption

  * Discuss this with team, maybe more people have the same assumption

### 3.6. Text Manipulation

* It takes time to master tools

* For shell users there are tools like `awk` and `sed` for faster scripting

* Using Python and Ruby can help you quickly hack up solutions

* Scripting languages can increase the rate of experimentation by 5 to 10 times

* **_Learn a Text Manipulation Language (Tip 35)_**

* Wide ranging applications of _Text Manipulation Languages_

  * Building the Book (generate PDFs, ebooks, etc)

  * Code inclusion and highlighting (inject code into book automatically from repos)

  * Website update (extraction of table of contents and injected into website)

  * Including equations (LaTeX math to nicely formatted text for the book)

  * Index generation (Indexes are marked up in text and then collated and formatted)

* Keeping things in text will bring a whole host of benefits

### 3.7. Engineering Daybooks

* Keep a daybook to:

  * Jot down what you are working on

  * Note variable values while debugging

  * Leave reminders where we put things

  * Record wild ideas

  * Sometimes just doodle (doodling helps focus and improves cognitive abilities)

* Advantages of keeping a daybook:

  * It is more reliable than (human) memory

  * It gives you a place to store ideas to work on later and focus on task at hand

  * It acts as a rubber duck, and helps you reflect your ideas and highlight mistakes

* Use paper, not a file or a wiki

* Wait a month and see the benefits

## 4. Pragmatic Paranoia

* **_You Can't Write Perfect Software (Tip 36)_**

* Did that hurt? It shouldn't! It is an axiom of life

* We can turn this to advantage

* We never put ourselves in a position from which we can't extricate ourselves

* We don't trust data and put assertions, look out for attackers etc

* Pragmatic Programmers take this a step further and don't trust themselves either

* Knowing that no one writes perfect code, build defenses against your own mistakes

### 4.1. Design by Contract

* > _Nothing astonishes men so much as common sense and plain dealing._
  > _--- Ralph Waldo Emerson, Essays_

* Clients and suppliers must agree on rights and responsibilities

* Dealing with computer systems is hard

  * Dealing with people is even harder

* But we have more data on how to deal with people since computers are newer

* One of the best solution for ensuring plain dealing is _contract_

* A contract defines your rights and responsibilities as well as of the other party

* In addition, there is an agreement concerning reprecursions

* Contract is an idea used over the world - both formally and informally - to help humans interact

* Same can be done to help software modules interact

* There are three parts of a DBC:

  * Preconditions: Caller of a routine is responsible for satisfying preconditions

  * Postconditions: The responsible routine must guarantee postconditions

  * Class invariants: These must hold true after the routine has finished

* If all the preconditions are met by the caller

  * The routine shall guarantee that all postconditions and invariants will be true

* If either party fails, a predecided remedy is invoked - maybe an exception or termination

* Failure to live upto the contract is a bug

* **_Design With Contracts (Tip 37)_**

* Write lazy code, accept specific inputs and output specific things

* DBC is needed even in a world of Test Driven Development

* In languages that do not have built-in DBC, you can code it in unit-tests

* Use assertions to partially implement DBC

  * It is partial because in OOP assertions are not automatically inherited

* It is mostly on code boundaries that most contract violation problems are detected

* DBC and Crashing Early

  * For e.g. `sqrt` function should crash if a _-ve_ number is given

* Semantic invariants are kind of a _philosophical contract_

  * The system is designed around these

* Sometimes software can update its contract at runtime, for e.g.

  * On recieving an invalid input, it might say

    * "I don't accept this, but if you give me that I might give you something else"

### 4.2. Dead Programs Tell No Lies

* Check things often and terminate the program if things go awry

### 4.3. Assertive Programming

* Write code that actively verifies your assumptions by checking along the way

### 4.4. How to Balance Resources

* As programs get more dynamic, system resources will be juggled

### 4.5. Don’t Outrun Your Headlights

* We stick to small steps so we don't fall off the edge of they cliff

## 5. Bend or Break

### 5.1. Decoupling

### 5.2. Juggling the Real World

### 5.3. Transforming Programming

### 5.4. Inheritance Tax

### 5.5. Configuration

## 6. Concurrency

### 6.1. Breaking Temporal Coupling

### 6.2. Shared State Is Incorrect State

### 6.3. Actors and Processes

### 6.4. Blackboards

## 7. While You Are Coding

### 7.1. Listen to Your Lizard Brain

### 7.2. Programming by Coincidence

### 7.3. Algorithm Speed

### 7.4. Refactoring

### 7.5. Test to Code

### 7.6. Property-Based Testing

### 7.7. Stay Safe Out There

### 7.8. Naming Things

## 8. Before the Project

### 8.1. The Requirements Pit

### 8.2. Solving Impossible Puzzles

### 8.3. Working Together

### 8.4. The Essence of Agility

## 9. Pragmatic Projects

### 9.1. Pragmatic Teams

### 9.2. Coconuts Don’t Cut It

### 9.3. Pragmatic Starter Kit

#### Ruthless and Continuous Testing

### 9.4. Delight Your Users

### 9.5. Pride and Prejudice
