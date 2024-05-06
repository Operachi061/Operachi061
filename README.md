# Description
Hobby programmer loving computers. 

# Strict example (may be changed)
```
--[[
    This is a Strict Language
    Big Example. 
]]--


$obtain("std"); 

setfun print_eight(int[unset:sig,64b,lock,fmt] string) int[unset:pub] {
    setvar end int[unset:nosig,16b,lock] = 4;
    assign new_end = end + 4;

    repeat -> x until (0 == new_end) {
        if (x == new_end - (1 + 2)) {
            <std>::printout("Loop: @d \nString: special text\n", /x/);
        } elseif (x == new_end - (1 + 1)) {
            <std>::printout("Loop: @d \nString: second special text\n", /x/);
        } else {
            <std>::printout("Loop: @d \nString: @s\n", /x/string/);
        }
    }

    return new_end;
}

setfun main() anyvar[unset:pub,err] {
    setvar world int[5:8b,nosig,lock] = "World";
    setvar returned_int int[unset:nosig,lock,16b] = print_eight("Hello @s!\n", world); 
    
    <std>::printout(returned_int);

    return new_return;
}

```


# About Me
https://operachi061.github.io/aboutme/
