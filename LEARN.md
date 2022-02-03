# if else

Solidity support conditional statements `if`, `else if` and `else`.  
It also supports a ternary operator.

## if else statement

Let's write a simple if else condition to return 0 if the value is less than 10 or 1 if the value is greater than 10 and less than 20 or 2 if the value is greater than 20.

Note the use of `else if` keyword to handle multiple conditions.

```
    function foo(uint x) public pure returns (uint) {
        if (x < 10) {
            return 0;
        } else if (x < 20) {
            return 1;
        } else {
            return 2;
        }
    }
```

Try to call ```foo``` and test the three cases.

## Ternary operator

Solidity supports a ternary operator which is a shorthand for an if-else statement.

Let's write a simple ternary operator to return 1 if the value is less than 10 or 2 if the value is greater than 10.

```
    function ternary(uint _x) public pure returns (uint) {
        // if (_x < 10) {
        //     return 1;
        // }
        // return 2;

        // shorthand way to write if / else statement
        return _x < 10 ? 1 : 2;
    }
```

Try this as well.
