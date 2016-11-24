#Analysis
There are **9 marks** available for this section.

##Introduction
In this section you must define **precisely** what your proposed system will do. To do this you will need to:

- Identify the client
- Describe the current system (if any)
- Define the problems with the current system 
- The users of the current system 
- The skill levels of the current users 
- Outline (multiple) possible solutions to solve these problems
- Describe possible problems with implementing each possible solution
- Identify what the system must do
- Realistically appraise possible solutions
- Select and justify a solution

The following sections will help you to produce a framework for your Analysis.

###Identify the client
Here you should describe who the system is for, what they do and what kind of organisation they work for. You should also explain why they have an interest in developing this system. In addition, make sure:

- that the role of the client is clear
- that you link the role of the client to the system that is going to be developed

###Describe the current system and define the problems.
In order to describe the current system effectively you will need to know more about it. You will do this by interviewing the client. During the interview you will also discover the problems with the current system.

You will need to at least one and possibly several meetings with your client in order to establish the detailed requirements for the project.

####The key to a successful interview is preparation.
Before you meet your client you should prepare a list of questions you want answered so that you are focused on getting the information required during your meeting. Never meet the client for a vague 'chat' as you will come away with more questions than answers!

In addition, give your client a copy of the questions ahead of time so that they can prepare effectively as well - this will make your meeting much more productive.

#####Interview checklist
This checklist of points may help you develop an appropriate set of questions for the interview:

Here is a checklist of points you may want to cover in an Interview:

- Objectives: what is the proposed system to do?
- What are the problems with the current way of doing things?
- What data or information is recorded in the current system?
- How much data is recorded at present?
- What data or information is to be recorded in the proposed system? How much data will the proposed system record?
- How frequently will the data need to be updated?
- Will new records need to be added or old ones deleted? How often?
- Will the changes come in batches or in ones and twos?
- How important is the data or information that is recorded?
- What processes or functions are performed by the current system?
- What processes or functions are to be performed by the new system?
- When should they be done and where?
- What special algorithms do these processes use?
- Which processes should be executed manually?
- What are the inputs to the current system?
- What inputs are required for the proposed system?
- What are the outputs from the current system?
- What outputs will be required from the proposed system?
- Are hard copies required?
- How often will outputs be required?
- What computing resources does the client possess?
- Is the client prepared to purchase hardware/software resources?
- Is security an issues?
- Should there be restricted access to particular areas?
- How are exceptions and errors handled in the current system?
- What errors and exceptions should be reported in the proposed system?
- How should they be reported?
- Are there any constraints on hardware, software, data, methods of working, cost, time, etc.?
- Does the user have a particular solution in mind?

####The purpose of the Analysis interview is not design.
During your initial interview with the client focus on discovering what the system is expected to do, **not** how it is supposed to do it. Leave discussions about the design and user interface until a later date - once you have a clear idea of the different inputs, processes and outputs of the system.

####Summarise
From the client interview you will be able to produce a summary which describes the current system and how it works, as well as defining and explaining the problems that the current system has. Keep in mind that it should be possible to **visualise exactly what the current system does** from your description - be as detailed as possible.

In relation to the problems you should clearly list and explain each problem. Make sure that you explain *why* each problem is an issue. Using bullet points to structure this section is helpful.

You should always include your original interview notes as an appendix to your document and look to get copies of any documentation from  the client that they use with the current system: order forms, invoices, letters etc. as these will be useful later on during the design stage.

##Investigation
This section should focus on describing both the **current** and **proposed** systems in detail. You should have separate sub-sections for each system.

###Data sources and destinations
This **table** should provide an overview of where the data for the system is coming from (source) and where it ends up (destination). You need to make sure that all data items are identified individually e.g. **first name**, **last name** etc. rather than just **name**.

Think carefully about both the sources and destinations - does the user pass data to the client directly or is there another destination e.g. a form.

The table should be structured in the following way:

|Source|Data|Example Data|Destination|
|----|---------|------|----------|
|User|Amended Patient Information|First Name|Receptionist|

###Algorithms
This section can be quite challenging as it is difficult to identify algorithms, especially in the current system. Keep in mind that all systems have algorithms, even if they are **manual systems**.

When you have identified some algorithms for your system you should attempt to express them in **pseudo-code** and provide any other annotation that you think is appropriate.

###Data flow diagrams
A data flow diagram (**DFD**) is a good way of summarising the sources and destinations of data and the processing that takes place. These diagrams show how data is **transformed** into information and what data needs to be stored.

A **DFD** will always have sources and destinations and generally the data will be **processed** at some stage in the system. Be sure to use the correct symbols (see **Chapter 48 Aspects of software development** Dynamic Learning) and to label all of the arrows appropriately. If required split the diagram up into sub-diagrams so that it is easier to understand the system.

###Forms
In this section you should include any example **forms**, **invoices** etc. that you have been provided with to help with your understanding of the system.

You should annotate these forms to explain why you are including them. 
Remember that they might help inform the design of your user interface later in the project.

###Data Dictionary
A data dictionary is a table that stores meta-data. It stores the names of data items (fields or variables), data types, length, validation criteria and other characteristics such as usage, physical representation, ownership, authorisation and security. It will also show which programs or modules read or write the data.

Below is an example of a data dictionary:

|Name|Data Type|Length|Validation|Example Data|Comment|
|----|---------|------|----------|------------|-------|
|SubjectRefCode|String|5 chars|5 digits, must exist|54821|Unique to each subject|
|CentreNo|Integer|4 bytes|10000 to 80000|12345|Unique to each centre|
|CandidateNo|String|4 chars|4 digits|2345|Unique to each candidate within a centre|
|CandidateName|String|25 chars||BLOGGs, Joe Fred|Full name, Surname in capitals, other names after comma|

###Volumetrics
Volumetrics is an assessment of the volume of data that a system will be required to process and store. 

For instance: 
- The system should be able to store 200 member records initially and cater for expansion to 1000 members. 
- The system only needs to process one sale at a time because...

##Objectives
Here you should produce bullet point lists which cover the objectives of the project.

- **General objectives** e.g. Clear and easy to use menu structure
- **Specific objectives** e.g. The user should be able to edit customer details
- **Core objectives** i.e. Those specific objectives that the system must do
- **Other objectives** i.e. Those specific objectives that it would be desirable for the system to do if there is enough time available.

For examples of objective setting see [Appendix - Objectives setting examples](#objectives) .

##Entity Relationship Diagrams
In this section you must produce diagrams which show the relationships between the data stores (entities) in the proposed system.

##Entity Descriptions
For each of the entities in your ER diagrams you should provide an appropraite entity description showing all **attributes** and **keys**.

##Object Analysis
You must produce an object analysis, which consists of three stages:

- Determine the objects in the problem domain
- Determine the relationships between the objects
- Determine the attributes and the behaviours of each object

###Determine the objects
Think about the the problem and identify possible objects. Examples of objects include: Book, Person, Order, Car.

###Relationship Diagrams
Once you have the objects you must determine the relationships between these objects. Refer to **pages 241-242** of A2 Bond for further details on this.

###Class Definitions
Finally you should define each class - what attributes does a particular class have? what methods will it require? Refer to **pages 242** of A2 Bond for an example.

##Other abstractions (Graphs)
Depending on your problem you may find it helpful to use other graphical representations to help aid understanding of the problem. This is difficult to discuss in general terms but if you think something could be better described in a graphical manner, discuss this with your teacher.

##Constraints
In any project their are various limitations that must be described:

- **Hardware** - what kind of hardware is available? How does this impact the project? What recommendations would you make if additional hardware is required?
- **Software** - state whether the client has stated any preferences or has it been left to you to choose
- **Time** - has the client given you a deadline or is it the project deadline set by your teacher?
- **Knowledge** - how does the user’s knowledge of IT constrain the project (if any)?
- **Access rights** - who will be allowed to use the various parts of the system?

##Alternatives and solutions
Look at the possible methods of solutions such as writing a program, customising a database or creating a spreadsheet or web application. List the advantages and disadvantages of each potential solution considering details such as user interface, data storage and manipulation. This should lead to a **justification of your chosen solution**.

## Mark Criteria

Analysis 

Level | Mark range | Description
------|------------|------------|
3     | 7 – 9 | Fully or nearly fully scoped analysis of a real problem, presented in a way that a third party can understand. 
||| Requirements fully documented in a set of measurable and appropriate specific objectives, covering all required functionality of the solution or areas of investigation.
||| Requirements arrived at by considering, through dialogue, the needs of the intended users of the system, or recipients of the outcomes for investigative projects. 
||| Problem sufficiently well modelled to be of use in subsequent stages.
2 | 4 – 6 | Well scoped analysis (but with some omissions that are not serious enough to undermine later design) of a real problem. 
||| Most, but not all, requirements documented in a set of, in the main, measurable and appropriate specific objectives that cover most of the required functionality of a solution or areas of investigation. 
||| Requirements arrived at, in the main, by considering, through dialogue, the needs of the intended users of the system, or recipients of the outcomes for investigative projects. 
||| Problem sufficiently well modelled to be of use in subsequent stages.
1 | 1 – 3 | Partly scoped analysis of a problem. 
||| Requirements partly documented in a set of specific objectives, not all of which are measurable or appropriate for developing a solution. The required functionality or areas of investigation are only partly addressed. 
||| Some attempt to consider, through dialogue, the needs of the intended users of the system, or recipients of the outcomes for investigative projects. 
||| Problem partly modelled and of some use in subsequent stages.



##Appendix

### <a name="objectives">Objectives setting examples</a>
#### Project A objectives | Example
These are the full set of objectives from a supermarket product recommendation system:
1. Show confirmation message when changes made to data
2. Users must find it easy to work through the system
3. Pictures should be stored within the database as long binary data
4. The system should be readable to all users
5. The system should not cause any perplexity
6. Random product ID generator should create a random and unique Product ID
7. The system should show any recommendation of the products, depending on the data produced by the algorithm
8. Secure logging in procedure

It is hard from the set of objectives above to actually understand what the project is intended to do. 

For example, it does not identify that the system is to have a checkout system and recommend products based on what the customer had in their basket. Issues such as calculating the total for a basket and being able to produce a receipt are not covered but were expected requirements from reading the problem background section.

Objectives 1, 2, 4 and 5 are not really objectives to measure the technical solution against for completeness.

Objectives 6 and 7 are beginning to look like suitable objectives but 'the algorithm' was not discussed in the analysis stage of this project and this is where it should have been defined. Due to the student not performing enough analysis into how the recommendation system was to work it can be seen why the student struggled to set a well-defined objective.


#### Project B objectives  | Example
These are a subset of the objectives from a quiz based on puzzles:

3. In order to help the user if they are unable to answer the question, a puzzle must be shown below the question.
    1.1. The answer must be calculated based on the randomly generated question and displayed on a grid of 16 squares.
1.2 The first 15 of the aforementioned squares must be saved as JPEG images and the 16th should be replaced with an empty square.
    1.3 The order of the 16 squares must then be randomised and presented to the user, below the exam question.
    1.4 If it is next to an empty square, the user must be able to move a tile by clicking on it.
    1.5 The user must be able to submit an answer, even if the puzzle has not been solved.
2. The questions should be from four different topics: real numbers, regular expressions, reverse Polish notation and finite state machines.
     2..1 For the real numbers topic, the user must be shown a mantissa and exponent, and asked to convert them to a fraction.
    2.2 The regular expressions questions should describe a string and request for the user to write a regular expression that matches this.
     2.3 An input string will be shown to the user, along with a finite state machine and the user must input the output string for the finite state machines topic.
    2.4 For the reverse Polish notation questions, a statement in the form of reverse Polish notation will be shown and the user will have to convert it to a denary value.


The objectives above are more detailed and clearly give well defined criteria that will help with the design of the solution, provide measures to test the technical solution against and to finally appraise against in the evaluation.