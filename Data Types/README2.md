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