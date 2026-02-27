Python is known as an "object oriented" programming language.

This means that everything in Python is an _object_. An _object_ is a "thing" that might contain:

1. Some type specific data
2. Some type specific functions that can operate on the data inside of the type

To see why this matters, consider that a store price and a country name might both seem like simple values -- but the operations that make sense for them are completely different. You can multiply a price by a quantity, but multiplying two country names makes no sense. Python uses _types_ to formalize this: the type of an object determines both what data it holds and what operations are available on it.

Let's start by re-creating our "Hello, world" variable `x` that we generated in the previous notebook.

<Talk about using types>

* Demonstrate how to find the split method using tab completion
* Use the `type` function to identify what type we are working with

<Talk about core Python types>

Since Python is an object oriented programming language, it helps to understand what the core Python types actually are and what they do.

* Numeric types -- integer vs float
    - "Obviously substantial amounts of economic data is stored as numbers -- Things like years, GDP, revenue, profit, etc... We want to be able to operate on this data in a Python native way."
    - Using Python to do calculator-like operations
    - Warning: Python uses `**` for exponentiation, not `^` like in math or Excel -- `^` means something else entirely in Python and will give you a wrong answer silently
    - Floor/modulus division
* String types
    - More and more data is being represented as textual data. Some estimates put the amount of text data at between 10 times and 100 times more than the amount of numeric data... As we begin to do economic analysis, we would be leaving a significant amount of data on the table if we only ever worked with numeric data.
    - Allows us to represent text in Python
    - Can "concatenate" strings or repeat them using `+` or `*`
    - String methods like `lower`, `upper`, `count`... Ask students to pause and investigate a few other methods
    - String formatting -- there are two approaches: f-strings (the modern, preferred approach) and the `.format()` method; cover both but emphasize f-strings
* Booleans
    - Most analyses that you will do involve using a subset of your data - This means that you need to be able to determine whether certain elements of your data meet the criteria that you're analyzing. Booleans allow you to do this by representing a value as True or False
    - Comparisons
    - Negation
    - Multiple comparisons


