# U.S. Constitution as Python Code

A creative technical representation of the United States Constitution using Python classes, functions, and data structures.

## Overview

This project presents the U.S. Constitution as executable Python code, transforming legal text into programmatic structures. Each article, section, and constitutional concept is represented using modern Python features including:

- **Dataclasses** for government entities (Representatives, Senators, Presidents)
- **Functions** for constitutional processes (elections, impeachment, legislation)
- **Classes** for institutional bodies (Congress, Supreme Court, Electoral College)
- **Enums** for categorization (branches of government, bill types)
- **Type hints** throughout for clarity and documentation

## Features

### Complete Constitutional Coverage
- All 7 original articles of the Constitution
- Full Article I with all 10 sections detailing Congressional powers
- Executive branch structure and presidential powers (Article II)
- Judicial system and federal courts (Article III)
- Interstate relations and federalism (Article IV)
- Amendment process (Article V)
- Federal supremacy and oaths (Article VI)
- Ratification requirements (Article VII)

### Visual Documentation
The repository includes Mermaid diagrams illustrating key constitutional processes:
- **Separation of Powers**: How the three branches interact and check each other
- **Legislative Process**: How bills become laws, including veto procedures
- **Impeachment Process**: Step-by-step flow from charges to potential removal
- **Amendment Process**: Both methods of proposing and ratifying amendments
- **Supremacy Clause Hierarchy**: The order of legal authority in the U.S.

## Example Code

```python
# Checking if someone is eligible to be President
@dataclass
class President:
    name: str
    age: int
    natural_born_citizen: bool
    years_resident: int
    
    def is_eligible(self) -> bool:
        return (self.age >= 35 and 
                self.natural_born_citizen and 
                self.years_resident >= 14)

# How a bill becomes law
class LegislativeProcess:
    @staticmethod
    def pass_bill(bill: Bill) -> "PassedBill":
        # Must pass both houses in identical form
        return PassedBill(bill)
```

## Structure

The main document (`us_constitution.md`) is organized by:
- **Articles** (I-VII) representing major constitutional divisions
- **Sections** within each article covering specific topics
- **Python code blocks** implementing constitutional concepts
- **Bullet points** summarizing key provisions

## Purpose

This project serves multiple goals:
1. **Educational**: Makes constitutional concepts more accessible to programmers
2. **Analytical**: Reveals the systematic structure of governmental design
3. **Creative**: Demonstrates how legal frameworks can be expressed as code
4. **Practical**: Shows type relationships and process flows in government

## Technical Requirements

- Python 3.7+ (for dataclass support)
- Type hints are used throughout
- No external dependencies required

## Contributing

This is a creative interpretation project. Contributions that enhance clarity, add missing constitutional elements, or improve the Python implementations are welcome.

## License

Public Domain - Like the Constitution itself

## Note

This is an educational/artistic project. For legal reference, always consult the actual text of the U.S. Constitution and appropriate legal resources.