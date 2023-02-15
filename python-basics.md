## Python basics

### What is a variable?

> A variable in Python is a memory location reserved for storing values. In other words, a variable in a Python program provides data to the computer for processing  

Variables in Python are declared like this:  

The variables in the editor are done like this (although in the console it can be done without the parentheses) you can also do subtraction, and so on  
And you can rename the variable as simple as this (yes, renaming the variable loses the previous value and happens to have another)  

````python
variable = 7

variable7 = 77

print(variable + variable7)

//(In this case the result would give 84)

variable = 777
````

> **Notice**: The identifier of a variable cannot start with a number and must be in lowercase. The words of the same are separated with an underscore  

And you can also create variables with the result of operations with other variables  

````python
variablex = variable + variable7
````

### Exploring Python: Arithmetic Operators

**Order of precedence**  

1. **Exponent**: `**`
2. **Negation**: `-`
3. **Multiplication, Division, Integer Division, Modulus**: `*`, `/`, `//`, `%`
4. **Addition, Subtraction**: `+`, `-`

### The primitives: simple data types

In programming, **a data type is the attribute that specifies to the computer the kind of data it has to handle**, in order to know what values it can take and what operations to perform. The most common primitive or elementary data types in programming languages are the following:  

- **Whole numbers** (and with negative sign)
- **Floating point numbers** (decimals)
- **Alphanumeric** (characters)
- **Character strings** (texts)
- **Logical states** (boolean)  

### Constants
A constant is a type of variable which cannot be changed. That is very helpful to think of constants as containers that contain information which cannot be changed later  

### Logical and comparison operators

A **logical operator** is used to make a decision based on **multiple conditions**. The **logical operators** used in **Python** are `and`,` or`, and `not`  

| Operator | Description                                 | Use     |
| :------  | :------------------------------------------ | :------ |
| and      | Returns true if both operands are true      | a and b |
| or       | Returns true if any of the operands is true | a or b  |
| not      | Returns true if its respective operand is false | not a |
|                                                        |         |

Comparison operators are used, as the name suggests, to compare two or more values. The result of these operators is always True or False  

| Operator | Description                                 |
| :------  | :------------------------------------------ |
| >        | Greater than. True if the operand on the left is strictly greater than the one on the right; False otherwise |
| >=       | Greater than or equal. True if the operand on the left is greater than or equal to the one on the right; False otherwise |
| <        | Smaller than. True if the operand on the left is strictly less than the one on the right; False otherwise |
| <=       | Less than or equal to. True if the operand on the left is less than or equal to the one on the right; False otherwise |
| ==       | Equals. True if the operand on the left is the same as the one on the right; False otherwise |
| !=       | Different. True if the operands are different; False otherwise |
|                                                        |

### Functions

-  **input()**: Allows **to obtain text typed ** by keyboard. Upon reaching the function, the program stops ** waiting for** something to be typed and the **Enter key** pressed

    ````python
    print ("What's yor name?")
    name = input ()
    ````

-  **int()**: Converts the specified value to an **integer**  

    ````python
    x = int (3.9)
    3
    ````

-  **str()**: Converts the specified value to a character **string**  

    ````python
    x = str(3.9)
    '3.9'
    ````

-  **len()**: Returns the **number of elements in an object**. When the object is a **string**, the len() function returns the **number of characters** in the string  

    ````python
    mylist = "Hello"
    x = len (mylist)
    5
    ````

-  **slice()**: Returns a **slice object**. Used to **determine** how to **cut a sequence**. You can specify where **to start the cut** and **where to end**. You can also **specify the step**  

    ````python
    a = ("a", "b", "c", "d", "e", "f", "g", "h")
    x = slice (2)
    print (a [x])
    ````

### Methods for variables of type text (String)  

- **`name.upper()`**: The `.upper()` method returns a string where **all characters** are in **uppercase**. Symbols and numbers are ignored  

- **`name.capitalize()`**: The `.capitalize()` method returns a string where the **first character** is in **uppercase**  

- **`name.strip()`**: The `.strip()` method **removes leading** (**leading spaces**) and trailing (**trailing spaces**) (space is the default initial character to remove)  

- **`name.lower()`**: The `.lower()` method returns a string where **all characters** are **lowercase**. Symbols and numbers are ignored  

- **`name.replace()`**: The `.replace()` method **replaces** a **specified phrase** with another **specified phrase**  

     - **Note**: All occurrences of the specified phrase will be replaced, if nothing else is specified  
         
        ````python
        string.replace ("oldvalue", "newvalue", 10)
        ````

### Python conditionals

**if** EXPRESSION: The **conditional `if` statement** is used to make **decisions**, it basically evaluates a **logical operation**, that's, an expression that gives **result**` True` or `False` , and **executes the following piece of code** as long as the **result is true**  

**elif** EXPRESSION: The sentence `elif`, means, **Otherwise If** the **conditional expression** is fulfilled, **the block of sentences followed** is executed

**else**: The `else` statement, means, **Otherwise** it is fulfilled **without evaluating any conditional** expression and **executes the block of followed statements**  

> **Tip**: To comment or uncomment the lines of code that we have selected, we have the key combination `Ctrl-k-c`, to comment, and` Ctrl-k-u`, to uncomment  

### Python functions

A function is a block of code that only executes when it's called. You can pass data, known as parameters, to a function. A function can return data as a result  

````python
def add (a, b):
     result = a + b
     return result
````

### Loop functions

-  **while**: We can execute a **set of statements** as long as a **condition is true**

    ````python 
    i = 1
    while i < 6:
    print(i)
    i + = 1
    ````

-  **for**: Is used to **iterate over a sequence** (which is a list, tuple, dictionary, set, or string). With the `for` loop we can **execute a set of statements**, once for **each element** of a list, tuple, set, etc  

    ````python 
    fruits = ["apple", "banana", "cherry"]
    for x in fruits:
        print(x)
    ````

-  **range()**: Returns a **sequence of numbers**, starting from 0 by default, incrementing by 1 (**by default**) and stopping **before a specified number**  

    ````python 
    x = range(6)
    for n in x:
        print (n)
    ````

#### Interrupt the cycles in programming

-  **break**: Used to **break** a` for` loop or a `while` loop  

    ````python
    for i in range (1, 9):
    if i> 3:
        break
    print (i)
    ````

-  **continue**: Is used to **end the current iteration** in a `for` loop (or a` while` loop) and continue to the **next iteration**  

    ````python
    for i in range (1, 9):
    if i == 3:
        continue
    print (i)
    ````

### Data structures

- **Lists**: Are used to **store multiple items in a single variable**. Lists are one of the 4 types of **built-in data** in Python that are used to **store data collections**, the other 3 are **Tuples**, **Set** and **Dictionaries**, all with different qualities and uses  

  -  **Methods**  
     - `**list.append(elmnt)**`: The `.append()` method adds an **element** to the **end of the list**
     - `**list.extend(iterable)**`: The `.extend()`  method **adds** the **specified list items** (or any iterable) to the end of the current list  
     - `**list.insert(pos, elmnt)**`: The `.insert()` method inserts the **specified value** at the **specified position**
     - **`list.remove(elmnt)`**: The `.remove()` method **removes the first occurrence** of the element with the **specified value**  
     - **`list.pop(pos)`**: The `.pop()` method **removes the element** at the **specified position**  
     - **`list.clear()`**: The `.clear()` method **removes all** the **elements of a list**  
     - **`list.index(elmnt)`**: The `.index()` method **returns the position at the first occurrence** of the specified value
     - **`list.count(value)`**: The `.count()` method **returns the number of items** with the specified value  
     - **`list.sort(reverse = True | False, key = myFunc)`**: The `.sort()` method sorts the **list in ascending order** by default (difference between lowercase and uppercase). You can also create a function to decide the sort criteria  
     - **`list.reverse()`**: The `.reverse()` method **reverses the order** of sorting the elements
     - **`list.copy()`**: The `.copy()` method **returns a copy** of the **specified list**  

- **Tuples**: May **look like lists**, they're often used in different situations and for different purposes. Tuples are **immutable** and typically contain a **heterogeneous sequence of items** that are accessed by unpacking or **indexing**. Lists **are mutable**, and their elements are **normally homogeneous** and are accessed **by iterating on the list**  

````python
thistuple = ("apple", "banana", "cherry")
print (thistuple)
````

- **Dictionaries**: They're sometimes found in other languages like "**associative memories**" or "**associative arrays**". Unlike sequences, which are indexed using a numeric range, dictionaries are **indexed with keys**, which can be **any immutable type**; **strings** and **numbers** can always be keys. **Tuples can be used as keys** if they only contain **strings, numbers or tuples**; if a tuple contains any **mutable directly or indirectly** object, **it cannot be used as a key**  

````python
thisdict = {
   "brand": "Ford",
   "model": "Mustang",
   "year": 1964
}
````

  -  **Methods**  
      - **`dictionary.keys()`**: The `.keys()` method returns a **view object** that **contains the dictionary keys**, as a list  
      - **`dictionary.values()`**: The `.values()` method returns a **view object** that **contains the dictionary values**, as a list  
      - **`dictionary.items()`**: The `.items ()` method returns a **view object** that **contains the dictionary key-value pairs**, as tuples in a list


### Your first program: currency converter

### Building the path of a program with conditionals

### Multiple countries in my currency converter

### Modularizing our currency converter

Once the functions and parameters have been learned, it is time to put them into practice to improve the code we write in our currency converter  

But before we move on to do it we need to learn something new:  

- Many times the result of a function, when we finish executing a function, we want to save what the function returns in a **variable**. To do so we must:  

````python
    def sum (a, b):
        print ("Add two numbers")

    result = a + b

    return result # means returns and allows us to return the variable

    sum = sum (1, 4)

    print (sum)
````

Once this new concept has been explained, we can proceed to improve our currency converter:  

````python
    def converter (currency_type, euro_value):
        currency = input ("How many" + currency_type + "do you have ?:")

        currency = float (currency)

        euro = currency / euro_value

        euro = round (euro, 2)

        euro = str (euro)

        print ("You have $" + euro + "euros")

    menu = """
    Welcome to the currency converter

    1 - Dollars
    2 - Colombian pesos
    3 - Mexican pesos

    Choose an option: """

    option = int (input (menu))

    if option == 1:
        converter ("dollars", 1.3)
    elif option == 2:
        converter ("Colombian pesos", 4424)
    elif option == 3:
        converter ("Mexican pesos", 24)
    else:
        print ("Please enter a correct option")
````

> The best thing is to put our functions above our code, since if they are below they will not be carried out  
>

📌 ** SUMMARY: ** when using the functions we can create more than one parameter inside them, for this we have to place the name of the parameters that we are going to use and separate them by a comma. When working with these parameters we must be careful with the type of data that we are using, since these will allow us to work in one way or another. If we want the operations that we have inside a function to be stored inside a variable, we use `return` at the end of the function, we must also save the result of this function inside a new variable. It is preferable that the functions are always placed at the top of our code, since if they are very low they will not be executed  

### **Project: palindrome**

Once we have learned how to use functions within Python and how to modify strings. Now we must put all the knowledge into practice with a new program. Let's create a palindrome  

A palindrome is a word that is read the same way backwards and forwards  

To make our program we must:  

- Create a main function, this is a good practice since it will be the one that will run the program at the beginning. Whenever we are going to program we need to put a function at the beginning. The most used is `run`  

````python
    def run ():
        pass
````

- Place the entry point

````python
    if __name__ == "__main__": # This is the entry point of a Python program, once Python finds it it starts running the code below.
        run ()
````

- Implement the functions:

````python
    def palindrome (word):

        word = word.replace ("", "") # Replaces all space characters with nothing, that is, removes spaces.

        word = Loops word.lower () # Convert the string to lowercase
        
        word_inverted = word [:: - 1] # Change the order of the string by inverting it
    
        if word == inverted_word: # Identifies if the word is equal to the inverted word
            return True
        else:
            return False

    def run ():
        word = input ("Write a word:")

        es_palindrome = palindrome (word)

        if es_palindromo = True:
            print ("It's palindrome")
        else:
            print ("Not palindrome")

    if __name__ == "__main__":
        run ()
````

> A good Python practice is to leave two spaces between each function and the entry point  
>

📌 ** SUMMARY: ** within the good practices when writing code in Python we have: create a main function that runs our `def run ():` program, have an entry point that refers to our main function (`if __name__ == '__main __': `) and leave two blank spaces between the functions we created and the entry point. The main function can have any name, but by convention the names `main` and` run` are used more  

### **Project: primality test**

To take advantage of all the knowledge that we have already acquired, we are going to create a primality test within Python  

To do this test we must know the concept of ** prime numbers. ** Within mathematics it is a simple and fascinating term  

🔢 A **prime number** is anything that can be divided only by itself and by 1  

The important thing is that we do the divisions in an integer way, that is, having quotient and remainder of the division, we will never have a remainder that is going to be equal to zero, only when we divide by 1 and by the same number  

Prime numbers help cryptography to improve the security systems we handle  

To generate the program in Python we use:  

````python
def is_prime (number): # We create a function to identify if a number is prime  

    counter = 0

    for i in range (1, number + 1): # We place the + 1 because the last parameter of the range function is not taken into account within the range  

        if i == 1 or i == number:
            continue # What this line means is that if i is equal to 1 or i is equal to the number we skip the line
        if number% i == 0:
            counter + = 1
        if counter == 0: # What we do is ask if the counter is equal to zero, that is, if dividing the number by all the numbers gave all the inaccurate divisions.
            return True
        else:
            return False

    def run ():
        number = int (input ('Write a number:'))
        if is_prime (number): # This is a function that we are going to create to determine whether or not the number is a prime number
            print ('It's prime')
        else:
            print ('Not prime')

    if __name__ == '__main__':
        run ()
````

> When we have the following in an if conditional: `if is_prime (number) == True:`. We can avoid putting the `== True`, since within Python it is optional to put it. Python understands that we are asking if the result of the function is true  
>

📌 **SUMMARY**: within Python we can have many ways to reach the same result, you should always look for the most readable way that optimizes the system. When working with conditionals that refer to functions if we want to ask a question using Booleans, we can omit placing the value True `if function () == True`, this because Python itself already performs this operation without having to put it  

### **Project: video game**

The skills we have at the moment are enough to program a lot of things  

The last practice that we will do in this module is to create a video game that is extremely easy to program  

The game that we are going to program is called "Guess the number". This game consists in that the computer will choose a random number between 1 and 100 and we will have to guess which number the computer chose. We will have to program the computer so that if we get it right it will tell us that we won, but if we fail it will tell us that the number we are looking for is larger or smaller. In this way we will be able to try numbers until we find the right one  

To create it we use:  

- Python module: this is a code package written by the people who created Python and that we have available to be able to execute functions already written by those people.
    
    To use them we use:
    

````python
import random # Python's random module contains functions to work with the randomness of the language, that is, we can generate random data.
````

Once that is explained we can program our game:  

````python
import random

def run ():
random__number = random.randint (1, 100) # with the dot we access the functionalities of a different module. randint () generates a random number ranging from number a to number b.  

chosen_number = int (input ('Choose a number from 1 to 100:'))  

while chosen_number! = random_number:
    if chosen_number <random_number:
        print ('Find a larger number')
    else:
        print ('Find a smaller number')
        number_elegido = int (input ('Choose another number:')) # This request for a new number does not have to be inside else, if it is, it generates a loop
        print ('You won!')

if __name__ == '__main__':
    run ()
````

📌 **SUMMARY**: Within Python we have already seen that there are modules that are already loaded by the program, but we can also import new modules to use within our programs. For this we use `import module_name` at the top to import it and be able to use it. The random module allows us to work with random terms. We can access them using `random.randint (#, #)`  

### **Project: password generator**

Now we will put into practice all the knowledge that we have learned. For this we are going to create a **password generator**  

Many times when being in a browser and registering on a website, the browser usually suggests automatically generated passwords. This is a function of the latest generation browsers that what it does is fill in a password automatically  

This function we are talking about can be generated without problem with everything we've learned so far  

````python
import random

def generate_password ():
    uppercase = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L' , 'M', 'N', 'Ñ', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'X', ' AND Z']
    lowercase = ['a', 'b', 'c', 'd', 'e', ​​'f', 'g', 'h', 'i', 'j', 'k', 'l' , 'm', 'n', 'ñ', 'o', 'p', 'q', 'r', 's',' t ',' u ',' v ',' x ',' and Z']
    numbers = ['1', '2', '3', '4', '5', '6', '7', '8', '9', '0'] # The numbers must be in the format of text
    symbols = ['*', '+', '-', '/', '@', '_', '?', '!', '[', '{', '(', ')' , '}', ']', ',', ';', '.', '>', '<', '~', '°', '^', '&', '$', ' # ',' "']

characters = uppercase + lowercase + symbols + numbers # We will add all our lists in a single list
password = [] # We generate an empty list where we are going to put random characters to generate our password

    for i in range (15):
        character_random = random.choice(characters) # With the choice function of the random module we choose a random character from the entire list of characters
password.append(character_random) # What append does is append to the random character in password

password = "" .join(password) # This allows us to generate a string from our original list
return password # This allows us to save the password when executing the run function

def run():
    password = generate_password()
    print('Your new password is:' + password)

if __name__ == '__main__':
    run ()
````

> When we write code and name the files, the most common is to put the titles in English and all our code must be written in English.

> The letter ñ or ç is a character that can work on some systems and not on others, so it is recommended not to use it  


📌 **SUMMARY**: It is preferable that the language we use when writing code within Python and when naming our Python files is English, since this programming language seeks to assimilate to the English language. There are many methods within the random module that we learned, we can find them researching on the internet and with practice. When creating lists, we can create lists that are empty and then fill them with blocks of code. The `return` option is very good and helps us to save the data we made in the final variable  
