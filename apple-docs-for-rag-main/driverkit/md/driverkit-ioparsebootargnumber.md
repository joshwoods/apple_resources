

- DriverKit
-  IOParseBootArgNumber 

Function

# IOParseBootArgNumber

Parses any boot arguments in the macOS kernel boot-args.

DriverKitiOSiPadOSmacOS

``` source
bool IOParseBootArgNumber(const char * arg_string, void * arg_ptr, int max_len);
```

## Parameters 

`arg_string`  

C-string name of the argument.

`arg_ptr`  

Pointer to variable to received parsed value.

`max_len`  

Size in bytes of the argument pointed to by arg_ptr.

## Return Value

True if the argument was found and parsed successfully to arg_ptr.

## Discussion

If the named argument is present in the kernel boot-args, return its value as an integer.

## See Also

### Boot Support

IOParseBootArgString

Parses any boot arguments in the macOS kernel boot-args.

