# Ruby Bug: Unexpected Getter Method Behavior

This repository demonstrates an uncommon bug in Ruby related to how instance variables are handled when accessed via getter methods.  Attempting to assign a new value through the getter method does not modify the instance variable's internal value.

The `bug.rb` file showcases the problematic code. The `bugSolution.rb` file demonstrates a correct approach.

## Bug Explanation

In Ruby, getter methods provide read-only access to instance variables. Assigning a value to the getter method does not affect the actual instance variable. This is different from some other languages where a getter could act as a setter too.

## Solution

To modify an instance variable, you must use a setter method or assign directly to the instance variable within the class's methods.