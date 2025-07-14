

- DriverKit
-  IOParseBootArgString 

Function

# IOParseBootArgString

Parses any boot arguments in the macOS kernel boot-args.

DriverKitiOSiPadOSmacOS

``` source
bool IOParseBootArgString(const char * arg_string, char * arg_ptr, int strlen);
```

## Parameters 

`arg_string`  

C-string name of the argument.

`arg_ptr`  

Pointer to char array to received parsed value.

`strlen`  

Size in bytes of the char array pointed to by arg_ptr.

## Return Value

True if the argument was found and parsed successfully to arg_ptr.

## Discussion

If the named argument is present in the kernel boot-args, return its value as a c-string.

## See Also

### Boot Support

IOParseBootArgNumber

Parses any boot arguments in the macOS kernel boot-args.

