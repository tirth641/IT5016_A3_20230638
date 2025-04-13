# IT5016 Assignment 3 - [20230638]

## Project Overview
This project implements a simple requisition system where staff can request items, and the system calculates the total cost and determines if the requisition can be approved based on the total.

## Code Structure
- `requisitionsystem.py Part B`: Main Python script containing the logic for requisitions.
- `download/`: Folder for the final submission PDF.

## Design Principles Applied

### Single Responsibility Principle (SRP)
Each method in the `RequisitionSystem.py Part B class handles a specific task, such as collecting staff info, collecting requisition items, or processing approval.

### Open/Closed Principle
The logic for approval can be easily extended (e.g., different rules for different departments) without modifying existing functions.

### DRY (Don't Repeat Yourself)
The total calculation is centralized, and item storage uses a list for reusability. Could be enhanced further with custom item objects.

### Encapsulation
Attributes like `staff_id`, `total`, and `status` are encapsulated within the class, and accessed or modified through dedicated methods.

## Improvements
- Separate item handling into its own class (`Item`) for better OOP design.
- Use a JSON or CSV file to persist requisition data.
- Include exception handling and input validation (partially implemented).

## How to Run
```bash
python src/requisition_system.py
