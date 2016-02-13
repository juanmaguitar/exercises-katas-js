# Kata: Password Validation

### Problem Description

Create a function `passwordValidation()` that receives a string and returns `true` when:

- the string contains at least one letter in uppercase
- the string contains at least 2 numbers (digits)
- the string contains at least one of these special characters: $ # % & - ! ?
- the string has 10 characters or more

Otherwise the function should return `true`

### Stage 2 - `config` variable

Modify the previous function to use a variable called `config` being this one an object with the rules to apply in the validation.

This object should have the following structure:

    config = {
        size : 10,
        uppercase : 1,
        numbers : 2,
        special = "$#%&-!?"
    }

Modify the function to read the "rules" from this object,

After this modification the behaviour should be same (so the tests should pass the same)

### Stage 3 - `config` parameter

Modify the previous function to receive a second (optional) parameter that will overwrite the `config` variable if is passed to the function.

With this change we should be able to use our function with different rules specified in this (extra) parameter and also have a default behaviour if is not passed.




