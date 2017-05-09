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
