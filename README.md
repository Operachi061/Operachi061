# Description
Hobby programmer loving computers. 

# About Me
https://operachi061.github.io/aboutme/

# Strict example (may be changed)
```
--[[
    This is a Strict Language
    Big Example. 
]]--


!^[def num as 10]

$obtain("std");

setfun print_eight(int[unset:sig,64b,lock,fmt] string) int[unset:pub] {
    setvar end int[unset:nosig,16b,lock] = 4;
    assign new_end = end + 4;

    repeat -> x until (0 == new_end) {
        if (x == (new_end - 2) + 1) {
            <std>::printout("Loop: @d \nString: special text\n", /x/);
        } elseif (x == new_end - 1 + 1) {
            <std>::printout("Loop: @d \nString: second special text\n", /x/);
        } elseif (err != nil) {
            <std>::printout("Printout has an error");
        } else {
            <std>::printout("Loop: @d \nString: @s\n", /x/string/) >> err;
        }
    }

    return new_end;
}

setfun main() anyvar[unset:pub,err] {
    setvar world int[5:8b,nosig,lock] = "World";
    setvar returned_int int[unset:nosig,lock,16b] = print_eight("Hello @s!\n", world); 
    
    <std>::printout("Returned int: @d\n", /returned_int/);
    <std>::printout("Num: @d\n", /num/);

    return new_return;
}

```
