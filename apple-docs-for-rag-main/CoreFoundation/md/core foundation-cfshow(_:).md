

- Core Foundation
-  CFShow(\_:) 

Function

# CFShow(\_:)

Prints a description of a Core Foundation object to stderr.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFShow(_ obj: CFTypeRef!)
```

## Parameters 

`obj`  

A Core Foundation object derived from CFType. If `obj` is not a Core Foundation object, an assertion is raised.

## Discussion

The output is printed to the standard I/O standard error (stderr).

This function is useful as a debugging aid for Core Foundation objects. Because these objects are based on opaque types, it is difficult to examine their contents directly. However, the opaque types implement `description` function callbacks that return descriptions of their objects. This function invokes these callbacks.

### Special Considerations

You can use `CFShow` in one of two general ways. If your debugger supports function calls (such as `gdb` does), call `CFShow` in the debugger:

```
(gdb) call (void) CFShow(string)
Hello World
```

You can also incorporate calls to `CFShow` in a test version of your code to print out “snapshots” of Core Foundation objects to the console.

## See Also

### Miscellaneous Functions

func CFCopyDescription(CFTypeRef!) -> CFString!

Returns a textual description of a Core Foundation object.

func CFCopyTypeIDDescription(CFTypeID) -> CFString!

Returns a textual description of a Core Foundation type, as identified by its type ID, which can be used when debugging.

func CFGetTypeID(CFTypeRef!) -> CFTypeID

Returns the unique identifier of an opaque type to which a Core Foundation object belongs.

