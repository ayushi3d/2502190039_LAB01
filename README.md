# 2502190039_LAB01
# CS-1281: Machine Learning with Python Lab
## LAB 01 – SCRATCH STUDIO

**Course:** CS-1281 – Python Programming Lab  
**Branch:** Mechanical and Smart Manufacturing  
**Semester:** B.Tech 3rd Semester  
**Date:** 28 July 2026  
**Work Order:** 01 of 10  
**University:** Veer Surendra Sai University of Technology (VSSUT), Burla

---

# 1. OBJECTIVE

To understand fundamental programming concepts using Scratch and develop their equivalent Python programs. The lab focuses on user input, variables, conditional statements, loops, counters and basic machine simulation.

# 2. PROJECT A – NAME PLATE

**Scratch Project:** https://scratch.mit.edu/projects/1365020681

### Aim
To create an interactive Scratch program that asks the user for their name and branch and displays personalized welcome messages.

### Algorithm
1. Start the program.
2. Ask the user to enter their name.
3. Store the response in a variable.
4. Ask the user to enter their branch.
5. Store the branch name.
6. Display two personalized welcome messages.
7. Stop the program.

### Python Equivalent

```python
# Project A: Name Plate

print("===== NAME PLATE =====")

name = input("Enter your name: ")
branch = input("Enter your branch: ")

print("\nWelcome", name, "!")
print("Welcome to", branch, "Department!")

print("\nThank you for using Name Plate.")
```

### Sample Output

```text
===== NAME PLATE =====

Enter your name: Ayushi
Enter your branch: MSM

Welcome Ayushi !
Welcome to MSM Department!

Thank you for using Name Plate.
```

### Concepts Used
- Ask and Wait
- Variables
- User Input
- Answer Block
- Say Block

---

# 3. PROJECT B – QUALITY CHECK STATION

**Scratch Project:** https://scratch.mit.edu/projects/1365023862

### Aim
To simulate an industrial quality inspection station that checks manufactured parts and classifies them as accepted or rejected based on their quality values.

### Algorithm
1. Start the machine.
2. Ask the operator to enter the number of parts.
3. Repeat the inspection for each part.
4. Ask for the quality value of the part.
5. If the quality value is greater than or equal to 50, classify it as ACCEPTED.
6. Otherwise, classify it as REJECTED.
7. Display the inspection result.
8. Stop after all parts are inspected.

### Python Equivalent

```python
# Project B: Quality Check Station

print("===== QUALITY CHECK STATION =====")

parts = int(input("Enter number of parts to inspect: "))

for i in range(parts):
    print("\nInspecting Part", i + 1)

    quality = int(input("Enter quality value: "))

    if quality >= 50:
        print("Result: ACCEPTED")
    else:
        print("Result: REJECTED")

print("\nQuality inspection completed!")
```

### Sample Output

```text
===== QUALITY CHECK STATION =====

Enter number of parts to inspect: 3

Inspecting Part 1
Enter quality value: 75
Result: ACCEPTED

Inspecting Part 2
Enter quality value: 30
Result: REJECTED

Inspecting Part 3
Enter quality value: 90
Result: ACCEPTED

Quality inspection completed!
```

### Concepts Used
- For Loop
- If-Else Condition
- Variables
- User Input
- Machine Cycle

---

# 4. PROJECT C – PRODUCTION COUNTER

**Scratch Project:** https://scratch.mit.edu/projects/1365026698

### Aim
To develop a production monitoring system that counts accepted and rejected parts in a batch of 10 and calculates the acceptance percentage.

### Algorithm
1. Initialize accepted and rejected counters to zero.
2. Repeat the inspection process 10 times.
3. Enter the quality value of each part.
4. If the quality value is greater than or equal to 50, increment the accepted counter.
5. Otherwise, increment the rejected counter.
6. Calculate the acceptance percentage.
7. Display the total accepted parts, rejected parts and acceptance percentage.

### Python Equivalent

```python
# Project C: Production Counter

accepted = 0
rejected = 0

print("===== PRODUCTION COUNTER =====")

for i in range(10):
    quality = int(input(f"Enter quality value of Part {i+1}: "))

    if quality >= 50:
        accepted = accepted + 1
    else:
        rejected = rejected + 1

percentage = (accepted / 10) * 100

print("\n===== PRODUCTION REPORT =====")
print("Total Parts: 10")
print("Accepted Parts:", accepted)
print("Rejected Parts:", rejected)
print("Acceptance Percentage:", percentage, "%")
```

### Sample Output

```text
===== PRODUCTION REPORT =====

Total Parts: 10
Accepted Parts: 8
Rejected Parts: 2
Acceptance Percentage: 80.0 %
```

### Python Counter Logic

```python
accepted = 0
rejected = 0

for i in range(10):
    quality = int(input("Enter quality: "))
    if quality >= 50:
        accepted = accepted + 1
    else:
        rejected = rejected + 1
```

### Formula

Acceptance Percentage:

Acceptance Percentage = (Accepted Parts / Total Parts) × 100

### Concepts Used
- For Loop
- If-Else Condition
- Counter Variables
- Increment Operator
- Percentage Calculation

---

# 5. INSPECTION REPORT – PEER QUALITY CHECK

### Aim
To test the programs using different inputs and identify possible errors.

| Test Case | Input | Expected/Observed Behaviour |
|---|---|---|
| Silly Input | Letters instead of numbers | Numeric conversion fails with ValueError in Projects B and C. |
| Extreme Input | 999999 | Accepted because the value is greater than or equal to 50. |
| Empty Input | Press Enter without entering a value | Numeric conversion fails with ValueError in Projects B and C. |

### Conclusion of Inspection

The programs work correctly with valid numeric inputs. However, invalid or empty numeric inputs can cause runtime errors. This highlights the importance of input validation and exception handling in Python programming.

---

# 6. LEARNING OUTCOMES

After completing this lab, the following concepts were understood:

1. Creating interactive programs using Scratch.
2. Taking user input and displaying output.
3. Using variables to store information.
4. Implementing conditional statements using If-Else.
5. Understanding loops and repeated machine operations.
6. Using counters to monitor production.
7. Calculating acceptance percentages.
8. Identifying errors through software testing.
9. Understanding the relationship between Scratch blocks and Python programming.

---

# 7. CONCLUSION

This lab provided practical experience in developing basic programming logic using Scratch and Python. The three projects demonstrated user interaction, machine simulation, conditional decision-making and production monitoring. The inspection activity also highlighted the importance of input validation and exception handling.

---

# 8. PROJECT LINKS

| Project | Description | Link |
|---|---|---|
| Project A | Name Plate | https://scratch.mit.edu/projects/1365020681 |
| Project B | Quality Check Station | https://scratch.mit.edu/projects/1365023862 |
| Project C | Production Counter | https://scratch.mit.edu/projects/1365026698 |

---

# 9. STUDENT DETAILS

**Name:** Ayushi Srivastava  
**Registration Number:** 2502190039  
**Branch:** Mechanical and Smart Manufacturing  
**Semester:** B.Tech 3rd Semester  
**University:** VSSUT, Burla

**Course Instructor:** Lt. B. K. Barik

---
**END OF LAB 01**
