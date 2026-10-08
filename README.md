# IAI_SLE_03

# SLE-3: Architectural Design – Full C4 Model

**Course:** 02AML204 – Introduction to Artificial Intelligence  
**SLE:** 3 – Architectural Design (Full C4 Model)  
**Student:** Adarsh Ingale  
**PRN:** 25UAM083  
**Division:** B  

---

## 📌 Overview

This repository contains the SLE-3 architectural design work based on the **C4 Model**.

The objective of this SLE is to represent AI-agent architecture at four levels:

- **Level 1 – System Context**
- **Level 2 – Container**
- **Level 3 – Component**
- **Level 4 – Code**

Two AI agents are documented:

1. **Date and Time AI Agent**
2. **Advanced Calculator AI Agent**

---

# 1. Date and Time AI Agent

## 1.1 Description

The Date and Time AI Agent interprets date and time requests and returns the required temporal information or calculation.

### Main Features

- Current date and time
- Date addition and subtraction
- Date difference
- Day-of-week calculation
- Readable formatted output

---

## 1.2 C4 Level 1 – System Context

The user supplies a temporal request to the AI agent.

The agent:

1. Receives the request.
2. Parses the requested operation.
3. Performs the required calculation or retrieves the current local date/time.
4. Formats the result.
5. Returns the result to the user.

The **System Clock** is the external system used to obtain the current local time.

### Main Elements

- **User** – Provides the date/time request.
- **Date and Time AI Agent** – Processes the request.
- **System Clock** – Provides current local date/time.

---

## 1.3 C4 Level 2 – Container

The Date and Time AI Agent is divided into the following containers:

| Container | Responsibility |
|---|---|
| Input Module | Accepts date/time requests |
| Request Parser | Identifies operation, dates, times, and units |
| Date-Time Engine | Performs calculations and formatting |
| Output Module | Presents the final answer |

The Date-Time Engine can obtain the current time from the external System Clock.

---

## 1.4 C4 Level 3 – Component

The main components are:

- Input Handler
- Request Parser
- Date-Time Engine
- Validation / Calculation
- Output Formatter

### Operation Modules

- `get_current_datetime()`
- `add_or_subtract_date()`
- `calculate_date_difference()`
- Weekday lookup / day-of-week calculation

The parser selects the required operation, the engine performs it, and the formatter produces a readable response.

---

## 1.5 C4 Level 4 – Code Level

Important functions include:

```text
get_current_datetime()
parse_request(request)
calculate_date_difference(date1, date2)
add_or_subtract_date(date, value, unit)
format_result(result)
```

These functions represent the implementation-level responsibilities of the agent.

---

# 2. Advanced Calculator AI Agent

## 2.1 Description

The Advanced Calculator AI Agent accepts mathematical expressions and performs arithmetic and scientific calculations.

Depending on the implemented functions, it can support:

- Addition
- Subtraction
- Multiplication
- Division
- Powers
- Roots
- Percentages
- Trigonometric functions
- Logarithms

---

## 2.2 C4 Level 1 – System Context

The user enters a mathematical expression or calculation request.

The agent:

1. Receives the expression.
2. Validates the input.
3. Parses the expression.
4. Selects the required mathematical operation.
5. Evaluates the expression.
6. Handles errors.
7. Returns the result or an error message.

### Main Elements

- **User** – Enters the mathematical expression.
- **Advanced Calculator AI Agent** – Parses and evaluates the expression.
- **Result/Error Message** – Returned to the user.

---

## 2.3 C4 Level 2 – Container

The Advanced Calculator AI Agent contains:

| Container | Responsibility |
|---|---|
| Input Module | Receives the mathematical expression |
| Expression Parser | Identifies numbers, operators, parentheses, and functions |
| Calculation Engine | Performs arithmetic and scientific operations |
| Validation / Error Handler | Handles invalid input and mathematical errors |
| Output Module | Displays the result |

---

## 2.4 C4 Level 3 – Component

The main components are:

- Input Handler
- Expression Parser
- Operator Handler
- Scientific Function Handler
- Evaluation Engine
- Error Handler

### Operator Handler

Handles operators such as:

```text
+  -  *  /  ^  %
```

### Scientific Function Handler

Can handle functions such as:

```text
sin()
cos()
tan()
log()
sqrt()
```

### Error Handler

Handles problems such as:

- Invalid expressions
- Division by zero
- Mathematical errors

---

## 2.5 C4 Level 4 – Code Level

Important functions include:

```text
read_expression()
parse_expression(expression)
evaluate_expression(expression)
scientific_operation(value, operation)
validate_expression(expression)
display_result(result)
```

The functions separate input, parsing, validation, calculation, scientific operations, and result presentation.

---

# 3. Design Principles

The architecture follows a modular design.

### Separation of Responsibilities

Different tasks are assigned to different modules/components:

```text
Input
  ↓
Parser
  ↓
Validation
  ↓
Processing / Calculation
  ↓
Output
```

This makes the system easier to understand, test, maintain, and extend.

---

# 4. AI Contribution

AI tools may assist with:

- Code generation and refinement
- Test-case creation
- Documentation
- C4 architectural diagrams
- Understanding architectural concepts
- Function-level descriptions

The student remains responsible for:

- Selecting the required operations
- Reviewing the generated content
- Testing the system
- Verifying outputs
- Checking architectural consistency
- Explaining the final design

---

# 5. Repository Structure

A suggested repository structure is:

```text
SLE-3/
│
├── README.md
├── CONTRIBUTION_LOG.md
│
├── Date_Time_AI_Agent/
│   └── agent.py
│
├── Advanced_Calculator_AI_Agent/
│   └── calculator.py
│
└── diagrams/
    ├── context_diagram.png
    ├── container_diagram.png
    └── component_diagram.png
```

> The actual source-code and diagram filenames can be changed according to the files included in the repository.

---

# 6. Learning Outcomes

After completing this SLE, the student understands:

- What the C4 Model is.
- How to create a System Context diagram.
- How to identify containers in a software system.
- How to decompose containers into components.
- How to connect architecture with code-level functions.
- How modular architecture improves maintainability.
- How AI tools can assist in software architecture documentation.

---

# 7. Conclusion

SLE-3 demonstrates the architectural design of two AI agents using the complete C4 Model.

The **Date and Time AI Agent** focuses on temporal requests and date/time calculations, while the **Advanced Calculator AI Agent** focuses on mathematical and scientific calculations.

The four C4 levels provide a structured view from the overall system context to individual implementation functions. This makes the architecture easier to understand, communicate, test, and extend.

---

## 📄 Related Documentation

- `CONTRIBUTION_LOG.md` – Student contribution and AI contribution record.
- SLE-3 C4 Report – Complete architectural design and diagrams.
