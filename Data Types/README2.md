                            Condtionals

Conditional Statements:
    When writing code that performs differents actions for different decisions, conditional statements are used. There are 4 conditional Statement types:
            -The "if" conditonal specifies a block of code to be executed, if a specified condition is true.
            -"else" is used to specify a block of code , if the same condition is false. 
            -"else if" is used to specify a new condition to test, if the first condition is false.
            -"switch" is used to specify many alternative blocks of code to be executed.
    
    The way to write conditional syntax is like so: if (condition) {action to be done if condition is met}. 

    Again the "if" (all lowercase) is used to specify a block of code to be executed if the condition is true.
    Example:
        if (hour < 18) {
            greeting = "Good day";
        }
    
    Again, "else" condition specifies the code to be executed if the same condition is false.
    Example: 
        if (hour < 18) {
            greeting = "Good day";
        } else {
            greeting = "good evening";
        }
    
    Again, "else if" specifies a new condition if the first condition is false.
    Example: 
        if (time < 10) {
            greeting = "Good morning";
        } else if (time < 20) {
            greeting = "Good day";
        } else {
            greeting = "Good evening";
        }
    
    (Switch will be discussed in a later chapter).

Logical Operators:
    There are 4 logical operators in JS: || (OR), && (AND), ! (NOT) and ?? (Nullish). Logical operators can be used on any type of value (not only booleans).

    The || (OR) operator: only returns false if BOTH conditions are false. 
    Example:
        alert( true || true ); true
        alert( false || true ); true
        alert( true || false ); true
        alert( false || false ); false
    
    If an operand is not a boolean, it is converted to a boolean for the evaluation. 
   
    ** The OR operator is most commonly used in an if statement to test if "any" of the given conditions are true.
    Example: 
        let hour = 12;
        let isWeekend = true;

        if (hour < 10 || hour > 18 || isWeekend) {
            alert( 'The office is closed.' ); // isWeekend is true so it will alert().
        }
    FYI on The || (OR) operator:
        -It evaluates from left to right
        -Each operand is converted to a boolean. If the result is true, it stops and returns the originial value of that operand.
        -If all operands are false, it will return the last operand

    *Basically, if there is a true condition, the OR operator will return the first true; if there are no true conditions, the last operand will be returned.


    The && (AND) operator:  only returns true if BOTH operands are true. 
    Example:
        // This is using the if conditional 
        let hour = 12;
        let minute = 30;

        if (hour == 12 && minute == 30) {
            alert( 'The time is 12:30' );
        }
    
    Here's what the && (AND) operator does:
        - Evaluates from left to right
        - For each operand, converts it to a boolean. If the result is false it stops and returns the original value of that operand.  
        - If ALL operands are true, it will return the LAST operand.

        
        The ! (NOT) operator: accepts a single argument and converts the operand to boolean type; and returns the inverse (opposite) value. 
        Example: 
            alert( !true ); // would be false
            alert( !0 ); // would be true

        The double !! (NOT) is often used to convert a value to boolean type
        Example:
            alert( !!"non-empty string" ); // would be true
            alert( !!null ); // would be false

        **The precendence of ! (NOT) is the highest of all logical operators and will always execute first.``