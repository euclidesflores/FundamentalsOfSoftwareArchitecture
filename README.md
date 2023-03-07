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

**Architecture decision:** Are rules for constructing systems. Answer the questions on how a system should be constructed? example: What layers are allowed to access the database? business layer? service layer?

**Design principles:** design principles are guidelines, architecture decisions are hard-and-fast rules. Example: what communication protocol should the developers use? gRPC? RPC? REST?

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
There are two types of connascence: static and dynamic

2. Types of connascence and difference:
* **Static:** Refers to the source code level coupling and is discoverable via static code analysis.
* **Dynamic:** Concerning runtime behavior.

Static connascence can be determined by simple code analysis, whereas dynamic connascence analyzes calls at runtime.

3. Connascence of Type (CoT)
Static connascence that refers to the common facility to limit variables and parameters to specific types.

4. Strongest form of connascence
Connascence of Identity (CoI) is a dynamic form of connascence that occurs when multiple components must reference the same entity.

5. Weakest form of connascence
Connascence of Name (CoN) is the most desirable form of connascence and is when multiple components must agree on the name of an entity.

6. Which is preferred within a code base—static or dynamic connascence?
Prefer static connascence to dynamic, static connascence can be using simple code analysis tools.

# Architecture Characteristics Defined

1. Three criteria that an attribute must meet to be considered an architecture characteristic
* Specifies a nondomain design consideration
* Influences some structural aspect of the design
* Is critical or important to application success

2. Explicit characteristic vs implicit.
Explicit characteristics appear in requirements documents and other specific instructions. Implicit characteristics are not specified in requirements documents but they are an important aspect of the design.




