# CONTRIBUTION_LOG.md

# SLE-3: Architectural Design (Full C4 Model)

**Course:** 02AML204 – Introduction to Artificial Intelligence  
**SLE:** 3 – Architectural Design (Full C4 Model)  
**Student:** Adarsh Ingale  
**PRN:** 25UAM083  
**Division:** B  

---

## 1. SLE-3 Objective

The objective of SLE-3 was to design and document the architecture of AI agents using the **C4 Model**. The report presents the architecture at four levels:

1. System Context – Level 1
2. Container Diagram – Level 2
3. Component Diagram – Level 3
4. Code Level Overview – Level 4

The report covers two systems:

- Date and Time AI Agent
- Advanced Calculator AI Agent

---

## 2. Student Contribution

### 2.1 Understanding the Problem

- Understood the purpose and functionality of the Date and Time AI Agent.
- Understood the purpose and functionality of the Advanced Calculator AI Agent.
- Identified the major inputs, processing steps, outputs, and external dependencies of both agents.
- Studied how the C4 Model represents a software system from high-level context to implementation-level functions.

### 2.2 Date and Time AI Agent

The Date and Time AI Agent was designed to handle:

- Current date and time
- Date addition and subtraction
- Date difference
- Day-of-week calculation
- Readable formatted output

The architecture was divided into:

- Input Module
- Request Parser
- Date-Time Engine
- Output Module
- System Clock as an external system

At component level, the design includes:

- Input Handler
- Request Parser
- Date-Time Engine
- Validation / Calculation
- Output Formatter
- Operation modules for current date/time, date arithmetic, date difference, and day-of-week calculation

### 2.3 Advanced Calculator AI Agent

The Advanced Calculator AI Agent was designed to support:

- Basic arithmetic
- Scientific functions
- Expression parsing
- Input validation
- Error handling
- Formatted results

The architecture was divided into:

- Input Module
- Expression Parser
- Calculation Engine
- Validation / Error Handler
- Output Module

At component level, the design includes:

- Input Handler
- Expression Parser
- Operator Handler
- Scientific Function Handler
- Evaluation Engine
- Error Handler

### 2.4 C4 Architecture Preparation

The following architectural views were prepared:

- Context diagrams showing the relationship between the user, AI agent, and external systems.
- Container diagrams showing the major internal modules.
- Component diagrams showing the internal components and their responsibilities.
- Code-level overviews identifying important functions.

### 2.5 Design Decisions

The design was kept modular by separating:

- Input handling
- Request/expression parsing
- Calculation and evaluation
- Validation and error handling
- Result formatting

For the Date and Time AI Agent, standard date/time library functions were considered appropriate for reliable calendar calculations.

For the Advanced Calculator AI Agent, expression parsing and evaluation were separated to make the system easier to test and extend. Validation was performed before evaluation so invalid expressions and mathematical errors could be handled clearly.

---

## 3. AI Contribution

AI tools were used as an assistance and refinement tool during the SLE-3 work.

### AI Assistance Included

- Understanding and explaining the C4 Model.
- Assisting with the structure of Context, Container, Component, and Code-level views.
- Suggesting suitable components and responsibilities.
- Assisting with documentation and report wording.
- Supporting the preparation of architectural diagrams.
- Helping identify suitable function-level descriptions.
- Suggesting test cases and edge cases for the proposed operations.

### Student Responsibility

The student was responsible for:

- Selecting the systems and operations to be represented.
- Understanding the generated suggestions.
- Reviewing the architecture.
- Checking that the diagrams match the intended system behavior.
- Verifying the functions and responsibilities.
- Making final decisions about the architecture and report.
- Explaining the architecture during submission or evaluation.

---

## 4. Work Summary

| Activity | Contribution |
|---|---|
| Problem understanding | Studied both AI agent requirements |
| C4 Model study | Understood all four C4 levels |
| Context Diagram | Identified users, systems, and external dependencies |
| Container Diagram | Identified major modules |
| Component Diagram | Identified internal components |
| Code Level | Listed important functions |
| Design Decisions | Defined modular separation of responsibilities |
| Documentation | Prepared explanations and report content |
| AI Assistance | Used AI for refinement, documentation, and diagrams |
| Verification | Reviewed architecture and consistency |

---

## 5. Final Outcome

The SLE-3 work produced a complete C4-based architectural design for:

1. Date and Time AI Agent
2. Advanced Calculator AI Agent

The final architecture demonstrates how a user request moves through input handling, parsing, processing, validation/evaluation, and output generation.

The C4 model helped maintain consistency from the system context down to the implementation-level functions.

---

## 6. Declaration

I confirm that I reviewed and understood the architectural design prepared for this SLE-3 activity and verified the final diagrams, component responsibilities, and function descriptions before submission.
