# Missing begin chapter 11 notes

### Steps for developing user interfaces
1. know your user
    1. level of knowledge and experience
        * computer literacy
        * System experience
        * Experience with similar applications
        * Eductaion
        * Reading level
        * typing skill
    2. physical characteristics
        1. Age
        2. gender
        3. handedness
        4. physical handicap
    3. characteristics of user's taks and jobs
        1. type of use(discretionary/mandatory)
        2. frequency of use
        3. turnover rate for employees
        4. importance of task
        5. repetitiveness of task
        6. training anticipated
        7. Job category (exec/mangager/professional/secretary etc)
    4. psychological characteristics of the user
        1. probable attitude toward job
        2. probable motivation
        3. cognitive style
            * verbal or spatial
            * analytic or intuitive
            * concrete or abstract
2. understand the purpose of the user interface in terms of the applications overall purpose.
3. understand the principles of good screen design
    1. consistency among screens
    2. anticipate where the user will usually start
    3. apply a hierarchy to emphasize order of importance
    4. apply principles of pleasing visuals ( balance, symmetry, regularity, predictability, simplicity, unit, proportion, economy)
4. select the appropriate kind of window
    1. property window 
    2. dialog window
    3. message window
    4. palete window
    5. pop-up window
5. develop system menus
    1. provide a main menu (between 5 and 9)
    2. display all  relecant alternatives
    3. match the menu structure to the structure of teh application's tasks
    4. minimize number of menu levels
6. select the appropriate device-based controls (the physical means by which the user communicates their desires with the application joysticks, trackballs, graphics tablet, touch screens, mouses, microphones and keyboards)
7. select the appropriate screen-based controls (icons, buttons, text boxes, radio buttons) between 5 and 9 or organized into groups
8. organize and layout the window
9. choose appropriate colors


### Case tools for requirements
* graphical tool for drawing data flow diagrams
    * easier to change a diagram stored in CASE tool than to redraw
    * Details of teh product are stored in the CASE tool so the documentation is always available and updated
    * Not always user friendly
    * Almost impossible to program computer to draw as pleasing a diagram as a human
    * expensive 


### Other case tools for requirements
* text editor
* Survey construction tool
* Screen generator (for rapid prototype)

### challenges of the requirements phase
* employees of teh client organization often feel threatened by computerization
* The requirements team members must be able to negotiate
    * the client's needs may have to be scaled down
* Key employees of the client organization may not have the time for essential in-depth discussions
* Flexibility and objectivity are essential


# chapter 12
### specification document
* serves as contract between clienct and developer
* must be clear and understandable by the client
* must be complete and detailed for the design team
* specifies exactly what the product is to do
* Describes the constraints of teh system
* Describes acceptance criteria
* Help team select solution strategy

### constraints
1. timing
2. storage
3. security
4. Response time
5. portability
6. reliability
7. parallel running
8. deadlines

### acceptance criteria
* set of series of tests which can be used to prove the product satisfies the specifications
* indicates the developer's job is completed
* may be restatements of the constraints
* may be 

### solution strategy
* general approach to building the product
* Records are maintained of discarded strategies and why there were discarded (This will help if teh team must justify to SQA why they selected the method they did. it will also aid during maintenance)

### specification document writing techniques
* internal methods
    * natural language easy to learn
    * easy for client to understand
    * Easy to incorporate ambiguities contradictions
* Semiformal methods
    * move precise than infromal
    * client can understand
    * cannot handle things
* Formal methods
    * most precise
    * REduce faults
    * support correctness proving
    * difficult to learn
    * almost impossible for client to understand
* Semiformal techniques
    * data flow diagram DFD- gane and sairsens graphical technique
    * problem statement language/ problem statement analyzer- computer aided technique
    * Structured analysis/design technique- box and arrow diagram language
    * software requirements engineering method SREM- useful for specifying real-time systems and embedded systems
    * entity relationships modeling- data oriented technique useful for specifying databases
## formal methods-easier to validate code
    1. finitre state machine FSM
    2. petri net- carl adam petri in 1962
    3. Z- formal specification language
    4. anna- formal specification language for ada
    5. vienna definition language VDL- based on denotational semantics
    6. Communicating sequential processes CSP- by hoare based on idea the project is a sequences of events
## finite state mahines FSM
* FA = (j,k,t,s,f) where
* j = finite nonempty set of states
* k = set of inputs
* T = transition function mapping JXK _> j
* S & J = the start state
* F = set of final states (F is a subset of J)

* Using a FSM, a specification is
    * easy to write down
    * easy to validate
    * Easy to convert into a design
    * Easy to convert into code automatically
    * More precise than graphical methods
    * Almost as easy to understand
    * Easy to maintain
* However
    * timing considerations are not handled

## petri net(get notes here)
* useful for concurrent processes and synchronization
* Nondeterministic
* C = (P,T,I,O)
* p = finite set of places
* t = finite set of transitions
* I = input function mapping T to bags of places
    * T -> P
* O = output function mapping T to bags of places
    * T -> P
* Four tokens: one in p1 two in p2 none in p3 and one in p4
    * reperesented by the vector (1,2,0,1)


## petri nets *missing info
* a transition is enabled if each of its input places has as many tokens in it as there are arcs from the place to that transition
* Tansis

## Z - formal specification language
* four sections
    * given sets (sets that need not be defined in detail), data types and constants
    * State Definition (schema - group of variable declarations together with a list of predicates that constrain the possible values of the variables)
    * Initial state- description of the system when first turned on
    * operations
* Analysis of Z language
    * easy to find fault in specification written in Z
    * Requires writer to be concise
    * Allows for proofs
    * Not too difficult to learn
    * Has decreased the cost of software development
    * Easy to rewrite the specifications into natural language for the client
    * Z is the most widely used formal specification language
    * has been used successfully especially in europe
* difficulties in using Z
    * the large and complex set of symbols
    * Training in mathematics is needed

### other formal techniques
* __Anna__
    * for ada
* __Gist refine__
    * Knowledge based
* __VDM__
    * uses denotational semantics
* __CSP(Communicating sequential processes)__
    * CSP specificatiosns are executable
    * Like Z, csp has a high squiggle factor

### comparison of classical analysis techniques
* formal methods are 
    * powerful but difficut to learn and use
* Informal methods have
    * little power but are esy to learn and use
* There is therefore a trad-off of ease versus power
__FIGURE 12.29__ 

### which analysis techniques should be used?
* it depends on the 
    * project
    * Development team
    * Management team
    * Myriad other factors
* It is unwise to ignore the latest developments

### testing during specification phase
* __walkthroughs__
* __inspections__
* __Correctness proofs__

### CASE tools
* graphical drawing tool for DFD or petri Nets
* Data dictionary
* Combined drawing tool and Data Dictinary ( and possibly a consistency checker)
    * analyst/designer
    * Software through pictures
    * System architect 

### Metrics
* __Size__- number of pages in the document
* __Quality__- measure the number of faults of each type found during inspection
* __Effort__- counts of files, data items and operations

### Challenges of classical analysis
* A specification document must be
    * informal enough for the client but
    * formal enough for the development team
* Analysis ("what") should not cross the boundary into design("how")
* Do not try to assign modules to process boxes of DFDs until the classical design phase


# Object Oriented analysis

### Object-oriented analysis (OOA)
* semiformal analysis method for use with the object-oriented paradigm
* The unified process is most often used
* Classes are extracted

### Analysis workflow of unified process:
* Two overall aims
    1. obtain a greater grasp of teh requirements
    2. Express the requirements in a form making design and implementation easier

### Types of classes in UP
1. Entitiy classes 
2. Boundary classes 
3. Control classes


### Entity class
* class which models information which is "long lived" in the product
    * examples:
        * Account class
        * Investment class
    * Denoted with
        * 406 figure 13.1

### Steps to extract entity class
1. Functional modleing (present scenarios for all the use cases)
2. Enitty class modeling (Determine entity class and attribues)
3. Dynamic modeling (determine the operation performed by or on each entity)

### Boundary class
* class which models the interaction between the software product and its actors
* Generally associated with input or output
* Denoted 
    * pg 406 figure 13.1

### Countrol Class
* Class which models complesx computations and algorithms
* Denoted
    * pg 406 figure 13.1

### CRC cards
* Class reponsibility collaboration cards __(CRC)__
* Completed for each class giving:
    * Name
    * Functionality (responsibility)
    * List of other classes it invokes (collaboration)

### Strength/weakness of CRC
* Strength:
    * Interaction of team members can note missing or incorrect fields (attributes or methods)
    * Relationship between classes is clarified
* Weakness
    * not useful if unfamiliarc with the domain of the problem

### Extracting Boundary Classes
* Each input screen
* Each output screen
* Each printed report


### Extracting Control Classes
* Each nontrivial computation
* Any complex algorithm

# Chapter 13

### Architectural Design
* Design at the highest level
* Designate the modules
* Decomposing the problem into managable units

### Selection of type of architecture
1. independent components
2. Virtual machines
3. Repository architectures
4. Layered architectures
5. Data flow architectures
6. Design patterns

### One method to select basic architectures
1. Develop mental model of the application at a high level
2. Decompose into the required components
3. Repeate the above process for each of the components

### Goals of Architectural Selection
1. Extension - ability to easily add features
2. Change - ability to easily adjust to changing requirements
3. Simplicity - easy to understand and implement
4. Efficiency - execution, compilation, size


### Decomposition
* Decompose the problems so that it can be managed as a series of smaller problems
* Goals of decomposition:
    1. Cohesion - amount of interation within a module (maximize)
    2. coupling - amount of interation between modules (minimize)

### Models- different perspectives or views of an application
1. Use Case Model
    * Collection of use cases to describe "do this"
        * Concept invented by jacobson
        * Identifiend by its name and by the type of user of the application called the actor
        * Consists of teh interation betweeen the actor and the application
    * tell what the applictaion is intended to do
2. Class model
    * Use of class diagrams to describe "with..."
    * Explain the building blocks used to construct the application
    * Sometimes called object models
    * To create:
        * Create domain classes from requirements analysis
        * Create and/or use existing framework classes
        * Create design classes specific to the application
3. Component Model
    * Collection of data flow diagrams
    * Dexcribe "how" the application is to do its work
    * Describe the way in which the application is to do its work in terms of moving data
    * Application is viewed as data flowing among processing units
4. State model
    * Collection of stat/transition diagrams
    * Describ "when" the application does its work
    * Divide the application into states so that the application is always in exactly one of these states

#### UML- Unified modeling Language
* Package- component of an architecture - collection of classes
* Abstract classes (those that cannot be instantiated into objects) denoted with italics
* Aggregation (inclusion of objects of one class by another) denoted with a diamond and the numeral at the end of the aggregation line denoted the number of object aggregated.
* Dependency ( method of the dependent class refers to the second class) denoted with a dotted line arrow

### Framework
* A collection of classes that are usable by several different applications

### Tools for design
* modeling tools
    1. Drawing 
    2. Jump directly from model to source
    3. Reverse engineering
    
### Metrics for design
* Number of entries and exits per module(package)
* Graph-theoretic complexity ( Number of modules) (Number of modules having at least one function call between them) + 1
* Data flow complexity


### Dtailed design
* process which follows the architectural design in which the large recognized components of the project are described in finer detail. (pseudo code the modules which resulted from teh architectural design)
* We may think of the architectural design process delineating the modules of a project and what cthey must perform.
* We may think of the detailed design as describing how each module will accomplish its task.

### Road Map for Detailed Design
1. Begin with architectural models
2. Introduce classes and design patterns that connect the architectural classes with the domain classes
3. Refine models for consistency and completeness
4. Specify class invariants
5. Specify methods with pre-post conditions, flowchharts, pseudo-code
6. Sketch unit test plans
7. Inspect test plans and design 
8. Release for implementation 

### Factors for deciding to reuse - Components when designing
* Is the component documented as well as the rest of the project? if not, can it be?
* How much customization of the component is required? 
* Has the component been tested to the same level as or more so than teh rest of teh project? if not, can it be?

## Methods for representing the detailed design
1. Dtailed sequence diagrams
2. ?
3. ?

### How to specify a class design
1. Gather the attributes listed in the SRS (Software REquirements Specification)
2. Add additional attributes required for the design
3. Name a method corresponding to each of the requirements for the class
4. Name additional methods required for the design
5. Show the attributes and methods on the object model
6. State class invariants (an assertion that remain true throughout the designated computation)

### How to specdify a function
1. note the section of the SRS or SDD that this function (method) satisfies. 
2. State what expressions the function must leave invariant
3. State the methods preconditions
4. State the methods postconditions 
5. Provide pseudocode or flowchart for the algorithm

### Flowchart
* Graphical representation of the steps in an algorithm.
* One of the oldest forms used to describe an algorithm
    1. Diamonds for decisions
    2. Rectangles for operations
    3. Arrow for flow

### Pseudocode
* Short, choppy statements describing the steps in an algorithm 
* Non-language specific 
* advantages
    1. easy to understand but can be precise enough to express the algorithm
    2. Can be inspected for correctness independent of a language
    3. Defect rates can be collected and used as a prdictor for defect rates in the product using historical data.

### Advantages of pseudocode or flowcharts for detailed design
1. Clarify algorithm
2. Impose discipline on the process of documenting
3. Provide additional level of inspection
4. Often decrease overall costs

### Disadvantages of flowcharts and pseudocode
1. Create another level of documentation to maintain. 
2. Introduce error possibilities in translating to code
3. May require tool to extract pseudocode or facilities for drawing flowchart

### Challenges of the design phase
* The design team should not do too much
    * The detailed design should not become code
* The design team should not do too little
    * It is essential for teh design team to produce a complete detailed design 
* We need to "grow" great cdesigners
* Potential great designers must be
    * Identified
    * Provided with a formal eduction
    * Apprenticed to great designers, and
    * Allowed to interact with other designers
* There must be a specific career path for tehse designers with appropriate rewards

#  IMplementation
* The process of translation the detailed design into code. (programming)
* Unnit implementation refers to coding the smallest part of the project which can be separately maintained. (classes or methods)

### Selection of a programming language
* Client requests
* Only one available
* Most suitable
    1. for the application
    2. for the environment
    3. for the 
    
### goals of implementation
1. Satisfy the requirements specified in the detailed design
2. Conform to standars
3. Document work
4. Maintain records of time, defects
5. Promote maintainability


### steps for implementation
1. Plan the structure of the cod (complete detailed design)
2. Self inspect the design or structure
3. Type in the code complying to standards
4. Self inspect your code
5. Compile 
6. Test

### Principle of sound implementation
1. Try to reuse already existing code if possible
2. Enfore intentions (code not to be used anywhere else in the application or to be used in other parts)


### Sound Programming Practices
1. Use consistent and meaningful variable names
2. Use prologue comments for each function giving input, actions, output, author and date, modification and date, files accessed, date tested and approved by
3. Use no more than one statement per line
4. Make good use of white space
5. Restric levels of nesting to three or four
6. Be consistent with indenting
7. Read in parameters instead of hardcoding constatns

### Principles of implementation
1. Use qualifiers like final, const, and abstract to enforce intentions
    1. Final classes can't be inherited from
    2. final methods cant be inherited from
    3. The value of final variables can't be changed
2. Make constants, variable, and classes as local as possible
3. Make members inaccessible if they are not specifically intended to be accessed directly
    1. Make attributes private. Access through puble accessor functions.
    2. Make methods private if they are for use only by methods of teh same class
4. Include examples in documentation.
5. List methods alphabetically rather than trying to finda calling order among them. (you may group private, protected, and public methods.)

### Hints for working with pointers
* Avoid using pointer parameters in C++ use references instedad
* Never return a pointer to a new heap reference in C++
* Collect your garbage (use delete() on unneded objects)

### Hints for working with functions
* avoid type inquiry. Use virtual functions instead
* Avoid C++ friend functions except when oviously beneficial.
* Be careful in overloading operators

### Hints on working with exceptions
* Catch only those exceptions you know how to handle
* If the present method cannot handle the exception, there has to be a handler in an outer scope that can do so.
* If you can handle part of the exception then handle and rethrow the exception for handling in the outer scope
1. Follow agreed-upon development process inspect
2. Consider introducting classes to encapsulate legal parameter values
3. Where error handling is specified by requirements, implement
4. For applications that must never crash, anticipate all possible implementation defects (use defaults)
5. Follow a consistent policy for checking parameters

### Programming Standards
* Increase readability
* Improve discipline
* Enhance portability

### Examples of programming standards
1. Naming Conventions
    1. Name with concatenated words
    2. Begin class names with capitals
    3. Begin variables with lowercase letters
    4. Capitalize constant names
    5. Begin the name of an instance variable of classes with the underscore
2. Documentation for methods
    1. preconditions
    2. postconditions
    3. what method does
    4. what parameters must be passed
    5. exceptions it throws
    6. reason for choice of visiblitiy
    7. ways in whcih instance variables are changed
    8. know bugs
    9. test description
    10. History of changes
3. Within methods
    1. Perform only one operation per line
    2. Try to keep the size to one screen
    3. Use parentheses within expressions even if they are not needed by the syntax
4. Documenting attributes
    1. Provide all application invariants
    2. State its purpose


### tools and Environments for Programming
* IDE (interactive Development Environment) used for allowing programmers to produce more code in less time
    * Drag-and-Drop facilities for forming GUI components
    * Graphical representation of directories
    * Debuggers
    * Wizards
    
### Defect Severity Classification
* Major - Requirements not satisfied
* Medium - Neither Major nor trivial
* Trivial - A defect that will not affect operation or maintenance

# Freebie chapter

### Why postdelivery maintenance is necessary
1. Corrective maintenance- correcting a fault 
    * analysis, design, implementation, documentation, or any other type of faults
2. Perfective maintenance - improving the effectiveness of the product
    * adding functionality make run faster, improve maintainability
3. Adaptive maintenance - change reacting to a change in the environment in which the product operates
    * Porting to a new compiler, OS , or hardware
    * Change in tax code
    * Change in zip code

### Facts about postdelivery maintenance
1. More time spent on postdelivery maintenance than any other activity
2. Approximately 67% of the product cost is maintenance cost
3. The most challenging of all aspect of software production
4. Incorporates aspect of all of the other workflows of the product
5. The most thankless development task

### Problems with postdelivery maintenance
1. Product may have not been developed with maintenance in mind.
2. Not considered glamorous but a drudgery
3. Task often given to beginners not the more seasoned programmers with experience
4. Must avoid creating more faults when correcting one

### Requirements for postdelivery maintenance programmers
1. Ability to locate cause of a fault
2. Ability to function without good documentation
3. Ability to maintain documentation of changes
4. Ability to perform regression testing
5. Ability to perform requirements analysis, design and implementation for adaptive or perfective maintenance
6. Ability to design test for new functionality added

### Management of postdelivery maintenance
1. Defect report file by user
2. Reports may be prioritized
3. Work given to programmer for repair
4. Results tested by SQA and documented
5. Make sure changes do not adversely affect further maintenance
6. Encourage client to avoid the moving target problem

### The reqrds of maintenance
* Maintenance is a thankless task in every way
    * maintainers deal with dissatisfied users
    * If the user were happy, the product would not need maintenance
    * The user's problems are often caused by the individuals who developed the product, not the maintainer
    * The code itself may be badly written
    * Postdelivery maintenance is despised by many software developers
    * Unlss good maintenance service is provided,, the client will take fuutre development business elsewhere
    * Postdelivery maintenance is the most challenging aspect of software production and the most thankless

### Ensuring maintainability
* Maintenance is not a one-time effort
* We must plan for maintenance over the entire life cycle
    * Design workflow -- use information-hiding techniques
    * Implementation workflow - select variable names meaningful to future maintenance programmers
    * Documentation must be complete and correct, and reflect the current version of every artifact
* During postdelivery maintenance, maintainability must not be compromised
    * Always be conscious of the inevitable further maintenance
* Principles leading to maintainablity are equally applicable to postdelivery maintenance itself

###  The problem of repeated maintenance
* the moving target problem is frustrating to the development team
* Frequent changes have an adverse effect on the maintainability of the product

### The moving target problem
* The problem is exacerbated during postedelivery maintenance
* The more changes there are 
    * The more cthe product deviates from its original design
    * The more difficult further changes become
    * Documentation becomes even less reliable than usual
    * Regression testing files are not up to date
    * A total reqrite may be needed for further maintenance 
* Apparent solutino
    * freeze the specification once they have been signed off until delivery of the product
    * After each request for perfective maintenance, freeze the specification for (say) 3 months or 1 year
* In practice 
    * The client can order changes the next day
    * If willing to pay the price, the client can order changes on a daily basis
* "he who pays the piper calls the tune" 

### warning 
* it is no use implementing changes slowly
* The relevant personnel are replaced
* Nothing can be done if the person calling for repeated chang has sufficient clout

### Special problems with object oriented maintenance
1. To understand an ovject, maintainer must understand the object's hierarchy
2. Polymorphism results in the same name could have different meanings
3. Changes in the base class will affect the children classes.

### Reverse engineering
* The process of re-creating the design document and possibly the specification document give the source code.
* Its need is du t othe amount of legacy code (code written 15-20 years ago but still in use) 
* Reengineering
    * reverse engineering, followed by forwared engineering
    * Lower to higher to lower levels of abstraction
* Restructuring
    * improving the product without changing its functionality
    * Examples:
        * Prettyprinting
        * Structuring code
        * Improving maintainability
        * Refactoring (XP, agile processes)
* What if we have only the executable code?
    * Treat the product as a black box
    * Deduce the specifications from the behavior of the current product 

### Case tools for postdelivery maintenance
1. Version control tool
2. Configuration control tool
3. Pretty printer
4. Graphic tools
5. Display class hierarchy
6. Defect-tracking tool (bugzilla)


