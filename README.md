# Fundamentals of Software Architecture
[Fundamentals of Software Architecture: An Engineering Approach by Mark Richards and Neil Ford](https://www.amazon.com/Fundamentals-Software-Architecture-Comprehensive-Characteristics/dp/1492043451/ref=sr_1_1?keywords=fundamentals+of+software+architecture+an+engineering+approach&qid=1678122286&sprefix=Fundamentals+of+softw%2Caps%2C191&sr=8-1)

# Self-Assessment Questions

## Introduction

1. Four dimensions that define software architecture

* Architecture decisions
* Architecture characteristics 
* Structure
* Design Principles

2. Difference between an architecture decision and a design principle

**Architecture decision:** are rules for constructing systems. They answer the questions on how a system should be constructed? example: What layers are allowed to access the database? only the business layer? only the service layer? or both?

**Design principles:** design principles are guidelines, architecture decisions are hard-and-fast rules. Example: what communication protocol should the developers use? gRPC? RPC? REST?

**Structure:** refers to the type of architecture style. Microservices? Layered (n-tiered)? Pipeline architecture style?


3. Core expectations of a software architect
* Architecture decisions
* Analyze the architecture (continually)
* Keep current with latest trends
* Ensure compliance with decisions
* Exposure and experience
* Business domain knowledge
* Interpersonal skills
* Understand and navigate politics


4. First Law of Software Architecture

>Everything in software architecture is a trade-off.


5. Second Law of Software Architecture

> Why is more important than how.


## Architectural Thinking

1. Traditional approach of architecture versus development
### Architect:
* analyzes business requirements
* defines architectural characteristics
* selects which architecture patterns and styles would fit the problem domain
* creates components

### Development team
* Create class diagrams from the artifacts created by the architect. 
* Create user interface screens
* Develop and test source code

This approach no longer works because of the physical and virtual barriers that this approach creates between the architect and the development team disconnecting the architect from the team. 

2. The knowledge triangle

* The stuff you know
Example: A java programmer knows the java language

* The stuff you know you don't know
Example: A java programmer can know what a programming language called Clojure exists, but the java programmer has never programmed in that language.

* The stuff you don't know you don't know
Example: the java programmer does not know what other frameworks, tools, libraries and languages exist.

3. Why is it more important for an architect to focus on technical breadth rather than technical depth?

For an architect it is more beneficial to know that five solutions exist for a particular problem that to have singular expertise in only one. Architects must make decisions that match capabilities to technical constraints.

4. Ways of maintaining your technical depth
* Do frequent proof of concepts
* Tackle some of the technical debt stories or architecture stories
* Work on bug fixes
* Do frequent code review


# Modularity

1. Meaning of connascence
>Two components are connascence if a change in one would require the other to be modified in order to maintain the overall correctness of the system
> -- Meilir Page-Jones

There are two types of connascence: static and dynamic.

2. Types of connascence and difference:
* **Static:** Refers to the source code level coupling and is discoverable via static code analysis.
* **Dynamic:** Concerning runtime behavior (execution time)

Static connascence can be determined by simple code analysis, whereas dynamic connascence analyzes calls at runtime.

3. Connascence of Type (CoT)

Static connascence that refers to the common facility to limit variables and parameters to specific types.

4. Strongest form of connascence

Connascence of Identity (CoI) is a dynamic form of connascence that occurs when multiple components must reference the same entity.

5. Weakest form of connascence

Connascence of Name (CoN) is the most desirable form of connascence and is when multiple components must agree on the name of an entity.

6. Which is preferred within a code base—static or dynamic connascence?

Prefer static connascence to dynamic, static connascence can be determined using simple code analysis tools.

# Architecture Characteristics Defined

1. Three criteria that an attribute must meet to be considered an architecture characteristic

* Specifies a non-domain design consideration
* Influences some structural aspect of the design
* Is critical or important to application success

2. Explicit characteristic vs implicit.

Explicit characteristics appear in requirements documents and other specific instructions. Implicit characteristics are not specified in requirements documents but they are an important aspect of the design.

3. Some examples of operational characteristic

* Availability
* Reliability
* Continuity
* Scalability

4. Some examples of structural characteristic

* Configurability
* Portability
* Localization
* Maintainability

5. Some examples of cross-cutting characteristic

* Authentication
* Authorization
* Accessibility
* Security

6. Which architecture characteristic is more important to strive for: availability or performance?

It depends. Architects should strive to design architecture to be as iterative as possible, understand the key domains goal and domain situation.

# Identifying Architecture Characteristics

1. Reasons to limit the number of characteristics an architecture should support

Supporting too many architecture characteristics complicates the system design and leads to greater and greater complexity.

2. True or false: most architecture characteristics come from business requirements and user stories?

False. Most architecture characteristics come from listening to the key domain stakeholders and collaborating with them to determine what is important.

3. The domain concern time-to-market is equivalent to what architecture characteristics? 

Agility, testability and deployability.

4. Scalability vs elasticity

Scalability measures the performance of concurrent users, elasticity measures burst of traffic.













