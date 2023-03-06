# Fundamentals of Software Architecture
[Fundamentals of Software Architecture: An Engineering Approach by Mark Richards and Neil Ford](https://www.amazon.com/Fundamentals-Software-Architecture-Comprehensive-Characteristics/dp/1492043451/ref=sr_1_1?keywords=fundamentals+of+software+architecture+an+engineering+approach&qid=1678122286&sprefix=Fundamentals+of+softw%2Caps%2C191&sr=8-1)

# Self-Assessment Questions

## Introduction

1. Four dimensions that define software architecture

* Architecture decisiones
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
Example: A java programmer can know what a programming language called Clojure exists, but the java programmer has never promgrammed in that language.

* The stuff you don't know you don't know
Example: the java programmer does not know what other frameworks, tools, libraries and languages exist.

3. Why is it more important for an architect to focus on technical breadth rather than technical depth?
For an architect it is more benefical to know that five solutions exist for a particular problem that to have singular expertise in only one. Architects must make decisions that match capabilities to technical constraints.

4. Ways of maintaining your technical depth





