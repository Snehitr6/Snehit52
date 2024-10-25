Overview
This Python program evaluates logical rules using an Abstract Syntax Tree (AST) structure. The rules consist of conditions based on user-defined data attributes such as age, department, salary, and experience. The program allows users to input their data and checks it against predefined rules, providing results based on the evaluations.

Features
Abstract Syntax Tree (AST): The program constructs an AST for rules, enabling efficient evaluation of complex logical expressions.
Logical Operations: Supports logical operations (AND, OR) and various comparison operators (>, <, >=, <=, =).
User Input: Prompts users to input their data, which can include age, department, salary, and experience.
Debugging Information: Outputs debug information during evaluation to illustrate how comparisons are made.
Requirements
Python 3.x
No external libraries are required.
How to Use
Clone or Download the Repository: Download the code files to your local machine.

Run the Program: Open a terminal, navigate to the directory containing the code, and 

Verify
Open In Editor
Edit
Copy code
python <filename>.py
Replace <filename> with the name of the Python file (e.g., rule_evaluator.py).

Input Data: The program will prompt you to enter the following:

Age (integer)
Department (string)
Salary (integer)
Experience (integer)
View Results: After entering the data, the program will evaluate the predefined rules and display the results for each rule as well as the combined result.

Code Structure
Classes
Node: Represents a node in the AST. Each node can be an operand or a logical operation (AND/OR).
__init__: Initializes the node with type, left and right children, and value.
evaluate: Evaluates the node based on the provided data.
Functions
create_rule(rule_string): Parses a rule string and creates an AST node.
combine_rules(rule_strings): Combines multiple rule strings into a single AST using OR operations.
evaluate_rule(ast, data): Evaluates the AST against the provided data.
get_user_input(): Collects user input for the required fields.
Main Execution
The main section of the code:

Verify
Open In Editor
Edit
Copy code
((age > 30 AND department = 'Sales') OR (age < 25 AND department = 'Marketing')) AND (salary > 50000 OR experience > 5)

Verify
Open In Editor
Edit
Copy code
((age > 30 AND department = 'Marketing')) AND (salary > 20000 OR experience > 5)
Creates ASTs for the rules.
Combines the rules into a single AST.
Evaluates the rules and prints the results.
Example Output
After running the program and entering the required data, the output will indicate whether the input data satisfies the conditions defined in each rule. For example:

Verify

Open In Editor
Edit
Copy code
Rule 1 Evaluation Result: True
Rule 2 Evaluation Result: False
Combined Rule Evaluation Result: True
Conclusion
This program provides a flexible and efficient way to evaluate complex rules against user-defined data using an AST structure. It can be easily extended to include more fields, operators, or logical constructs as needed. The debug information helps in understanding the evaluation process and can be useful for troubleshooting or enhancing the rules.


