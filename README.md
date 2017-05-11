#Rosanna Speller

This is where I put my codecamp notes

_LCText_ citation refers to the LaunchCode customized version of Runestone's _ThinkCsPy_ 

## Types of Error Messages

### ParseError:

A **ParseError** ususally is punctuation mistake such as missing comma, parenthese, or quotation mark. This is a kind of **Syntax Error**. (_LCText_).

Also remember to use a single apostrophe twice instead of quote marks instead of a the quoation mark key inside of a string. 
**Example:**
 user_name=input("What is your name?)
 print(user_name)

There is a missing quotation mark when asking for the user_name which causes a Parse Error.

**Example:**
Error:
 user_name=input("What is your "Given Name"?")
 print(user_name)

Correction:
 user_name=input("What is your ''Given Name''?")
 print(user_name)
### TypeError:

A **TypeError** occurs when combine incompatible objects of different types. This can often happen with mathematical operations between incompatible objects. 

**Example:**
 input_value="This is a string."
 print(input_value / 4)

Here we try to do vision with a string and an integer number, these are incompatible types.

**Example:**

    age=7
    print("I am", age+".")

There is an error because **age** is an "int" type so cannot be concatenated with **"."**, which is a "str" type. 

### NameError:

A **NameError** generally means that a variable has been used before it is assigned a value.  Often this can occur because of a spelling error (_LCText_).

**Example:**
 variable_name=6
 print(varable_name)

This contains a spelling error so "varable_name" is undefined.

### ValueError:


**Example:**
Let's say we have a program that looks like this:

```python
    age=input("What is your age?")
    age_int=int(age)
    print(age)
```

If we run this program and the user gives "dog" for their age this is what happens. 

>$ python valueerror.py 
>What is your age?dog
>Traceback (most recent call last):
>   File "valueerror.py", line 2, in &lt module &gt
>   age_int=int(age)
>ValueError: invalid literal for int() with base 10: 'dog'

## Functions

**Does a funtion have to have parameters?**

If the function is defined without a parameter and called without a parameter it will run.  If there is a parameter one place but not the other there are errors. 

Chris says:
>"No. A function may have 0 or more parameters, as decided by a programmer."

**What happens if we call a function without providing a value for one or more input parameters?**

There are errors when there are missing value or input parameters. Specifically we have a TypeError because the number of "arguments" (parameter values) doesn't match with the definition of the function. 

UNLESS you put default values for additional arguments.  

    **Example:**
``` python
    def add_two(a,b=0)
        return a+b
    print(add(2))
    >2
```

    Here b has default a default value of 0.  If it just said aa_two 
**Does a function have to return a value?**

No.

**What happens if we have a function that doesn't return a value, but we try to store a return value in a variable?**

The variable will have the "special value" of None.