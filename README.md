# Odin_Variables-Operators

Variables:
    Variables are like storage containers for data in code. There are three ways to create a variable: var, let, and const. 


Arithmetic Operators:
    A typical arithmentic operator operates on two numbers. The numbers can be literals, variables, or expressions.
Literals: let x = 100 + 34;
Variables: let x = a + b; 
Expressions: let x = (100 + 34) * a;
    FYI: The numbers are called the operands and the express between them is called the operator.

There are eight basic operators in JavaScript Arithmetic:
    + Addition
    - Subtraction
    * Multiplication 
    ** Exponentiation (raises the first operand to the power of the second operand. Ex. let x = 5, let z = x ** 2 (5 squared)... is 25).
    / Division 
    % Modulus (Remainder)
    ++ Increment
    -- decrement 

Operator Proceedure:
Like in traditional mathmatics, when coding using arthimetic operators, Multiplication and division has a higher precedence than addition and subtraction. An like school, the order of the proceedure can be manipulated but parentheses. 

Numbers:
    Numbers can be written with or without decimals. Extra large and extra small numbers can be written with scientific (exponent) notation: Example, let x = 123e5; // 12300000, let y = 123e-5 // 0.00123.

Integer/Floating Precision:
    Integers are accurate up to 15 digits. So: if you code,    let x = 999999999999999; // x will be 999999999999999. But, let y = 9999999999999999; // y will be 10000000000000000. The maximum amount of decimals is 17. 

    Floating point arithmetic is not always 100% accurate. So, instead of coding: let x = 0.1 + 0.2; // 0.30000000000000004 it would be more accurate to code: let x = (0.2 * 10 + 0.1 * 10) / 10; // 0.3. 

Adding Numbers and Strings: "binary", "urnary", "operand".
    FYI: The + operator is used for both addition and concatenation.
    Rule of Thumb:
        - Two numbers results in a number
            let x = 10; y = 20; z = x + y; // 30
        - Two strings results in a string concatenation
            let x = "10"; y = "20"; z = x + y; // 1020
        - Adding a number and a string results in a string concatenation
            let x = 10; y = "20"; z = x + y; // 1020
    If there is a mix of string and numbers, the code moves from left to right. So, if the first operand is a string, followed by a number and another number, the string and number get concatenated and then follows the rule down the code.
    Example:
        let x = 10; y = 20; z = "The result is: " + x + y; 
            The "string" first gets added to the x (the rule says it would be concatenated), making 10 now "10". When you add "10" to 20 (The rule says to concatenate) the result is 1020. 
    Example:
        let x = 10; y = 20; z = "30"; 
        let result = x + y + z; // 3030

Numeric conversion, unary +
    The plus + is used in two forms: binary (as used in the above examples); and urnary   The plus operator applied to a single value, doesn't fo anything to numbers. If the operand is not a number, the urnary + converts it into a number.                       Example: 
        let x = 1;
        alert(+x); // 1 
        
        let y = -2;
        alert(+y); // 2

        //Converts non-numbers
        alert( +true ); // 1
        alert ( +"" ); // 0

    The need to convert strings to numbers arises very often. Often when gathering sums of information. By default, the binary plus would add them as strings: 
    Example:
        let apples = "2"; oranges = "3";
        alert( apples + oranges ); // "23", (because the binary + concatenates strings)

    To treat them as numbers, they must be converted and then sum them.
    Example:
        let apples = "2"; oranges = "3";
        alert( +apples + +oranges ); // 5
        //The longer variant: alert( Number(apples) + Number(oranges) ); // 5