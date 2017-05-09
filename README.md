This is where I put my codecamp notes

_LCText_ citation refers to the LaunchCode customized version of Runestone's _ThinkCsPy_ 

##Types of Error Messages

###ParseError:

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
###TypeError:

A **TypeError** occurs when you use a function which expects a certain value type (ex. string, float, integer) and the value you try to put through the function is not of the proper type. This can also happen when you try to combine different value types which are incompatible. 

**Example:**
 input_value="This is a string."
 print(input_value / 4)

The input value here is a string and you cannot use a mathematical operator on a string.

**Example:**

    age=7
    print("I am", age+".")

There is an error because **age** is an "int" type so cannot be concatenated with **"."**, which is a "str" type. 

###NameError:

A **NameError** generally means that a variable has been used before it is assigned a value.  Often this can occur because of a spelling error (_LCText_).

**Example:**
 variable_name=6
 print(varable_name)

This contains a spelling error so "varable_name" is undefined.

###ValueError:



