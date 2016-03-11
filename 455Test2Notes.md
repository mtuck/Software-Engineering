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
* SEmiformal techniques
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


## petri nets
* a transition is enabled if each of its input places has as many tokens in it as there are arcs from the place to that transition
* Tansis
