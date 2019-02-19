<b>Exercise 1: Run the program on your system and see what numbers you get. Run the program more than once and see what numbers you get.</b>

The random function is only one of many functions that handle random numbers. The function randint takes the parameters low and high, and returns an integer between low and high (including both).

    >>> import random
    >>> random.randint(5, 10)
    >>> random.randint(5, 10)
    >>> random.randint(5, 10)
    To choose an element from a sequence at random, you can use choice:

<b>Exercise 2: Move the last line of below program to the top, so the function call appears before the definitions. Run the program and see what error message you get.</b>

    >>> repeat_name_printing('Alex', 'Seong')
    
    >>> def print_my_name(fname, lname=''):
    ...     print("My name is ", fname)
    ...     print("My full name is ", fname, lname)

    >>> def repeat_name_printing(fname, lname=''):
    ...    print_my_name(fname, lname)
    ...    print_my_name(fname, lname)


<b>Exercise 3: Move the function call back to the bottom and move the definition of print_my_name after the definition of repeat_name_printing. What happens when you run this program?   
    
    >>> def repeat_name_printing(fname, lname=''):
    ...    print_my_name(fname, lname)
    ...    print_my_name(fname, lname)

    >>> def print_my_name(fname, lname=''):
    ...     print("My name is ", fname)
    ...     print("My full name is ", fname, lname)

    >>> repeat_name_printing('Alex', 'Seong')


<b>Exercise 4: What is the purpose of the "def" keyword in Python?</b>

    a) It is slang that means "the following code is really cool"
    b) It indicates the start of a function
    c) It indicates that the following indented section of code is to be stored for later
    d) b and c are both true
    e) None of the above


<b>Exercise 5: Write a program to prompt for a score between 0.0 and 1.0. If the score is out of range, print an error message. If the score is between 0.0 and 1.0, print a grade using the following table:</b>

    def alex():
        print("David")
    
    def karen():
        print("Jacob")
    
    karen()
    alex()
    karen()

a) David Jacob karen alex karen
b) David Jacob David
c) Jacob David karen
d) Jacob Alex Jacob
e) David David David

<b>Exercise 6: Rewrite the weighted average computation(exercise 1 of Conditional Expression) by creating and using a function called compute_average which takes two parameters(eng and math).</b>

    Enter Egnlish score: 95
    Enter Math score: 85
    
    Total score: 227.5 
    Average score: 113.75

    Enter Egnlish score: 75
    Enter Math score: 85
    
    Total score: 160 
    Average score: 80.0

<b>Exercise 7: Rewrite the grade program from the previous chapter using a function called computegrade that takes a score as its parameter and returns a grade as a string.</b>

    Score   Grade
    >= 0.9     A
    >= 0.8     B
    >= 0.7     C
    >= 0.6     D
     < 0.6     F

    Enter score: 0.95
    A
    Enter score: perfect
    Bad score
    Enter score: 10.0
    Bad score
    Enter score: 0.75
    C
    Enter score: 0.5
    F
