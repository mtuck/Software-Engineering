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
