# Description
Hobby programmer loving computers. 

# Strict example (may be changed)
```
--[[
    This is a big example 
]]--


$obtain("std.st"); 

setfun print_three(int[unset:sig,64b,lock,fmt] string) int[unset:pub] {
    setvar end int[unset:nosig,16b,lock] = 4;
    assign new_end = end + 4;

    repeat -> x until (0 == new_end) {
        <std>::printout("Line @d: \nString: @s", x:string);
    }

    return new_end;
}

setfun main() anyvar[unset:pub,err] {
    setvar world int[5:8b,nosig,lock] = "World";
    setvar returned_int int[unset:nosig,lock,16b] = print_three("Hello @s!", world); 
    
    <std>::printout(returned_int);

    return new_return;
}

```


# About Me
https://operachi061.github.io/aboutme/
