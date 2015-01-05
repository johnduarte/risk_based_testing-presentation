# Risk Based Testing

---

Ryan Gard and John Duarte

July 25, 2014

![](images/error.jpg)

# Why Risk Based Testing

---

- We cannot *Test all the things!*
- Test the **right** things
- Establishing the best priorities


# Defining Risk

---

Customer loss of value due to defect

- Severity
    - Impact to customer
- Probability
    - Likelihood of occurrence
- Unknown Qualities
    - Is the risk understood?

# Feature Analysis

---

Finding the surface area

# User Interface Identification

---

How can a user interact with the product?

# Input Enumeration

---

What are the possible inputs for each interface?

# Output Enumeration

---

What are the channels for outputs?

- User interfaces (stdout, stderr, GUI widget)
- Side effects (trigger processes, alter file system)
- Exit code
- Logging

# Input to Output Mapping

---

Each input must have one or more output in order to test it

# Configuration Enumeration

---

What are the external components that can impact the system?

# Test Case Enumeration

---

For each configuration value, exercise an Input to Output mapping


# Slice 'N Dice

---

Identify the **Right** things to test

What metrics do we use?


# Risk Levels

---

- High
    - High Severity AND
    - High Probability

- Medium
    - Moderate Severity AND
    - Low Probability

- Low
    - Low Severity AND
    - Low Probability


# Configuration Priority

---

Based on business concerns

- Most valuable markets (e.g. RHEL, Ubuntu)


# Resource Constraints

---

- Time
- Man Power
- Efficiency


# Case Sizing

---

- Complexity
- Cost of Execution


# Scoping In

---

1. Start with nothing
2. add *High Risk*
3. add *High Configuration Priority*
4. repeat until capacity is full OR *Highs* are exhausted


# Scoping Out

---

1. Start with everything
2. remove *Low Configuration Priority*
3. remove *Low Risk*


# Derivative Cases

---

Only for work in scope!


# Negative

---

- Invalid Data
- Data Boundary Violation
- State Transition Violation
- Mutually Exclusive Input
- Invalid Configuration

# Multi-Factor

---

Combined Input Cases


# Edge

---

Single Variable

> This one goes to eleven!


# Corner

---

Multiple Variables

> The numbers all go to eleven. Look, right across the board, eleven, eleven, eleven and...


# Attack

---

Outside of the defined User Interface


# Middle Ground

---

What to do with the cases that are neither in or out??



# Conclusion

---

- Beware of the Gotchas!
- Read the Docs on Confluence
