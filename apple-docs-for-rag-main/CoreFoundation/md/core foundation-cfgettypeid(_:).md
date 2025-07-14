

- Core Foundation
-  CFGetTypeID(\_:) 

Function

# CFGetTypeID(\_:)

Returns the unique identifier of an opaque type to which a Core Foundation object belongs.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFGetTypeID(_ cf: CFTypeRef!) -> CFTypeID
```

## Parameters 

`cf`  

The CFType object to examine.

## Return Value

A value of type CFTypeID that identifies the opaque type of `cf`.

## Discussion

This function returns a value that uniquely identifies the opaque type of any Core Foundation object. You can compare this value with the known CFTypeID identifier obtained with a “GetTypeID” function specific to a type, for example CFDateGetTypeID(). These values might change from release to release or platform to platform.

## See Also

### Miscellaneous Functions

func CFCopyDescription(CFTypeRef!) -> CFString!

Returns a textual description of a Core Foundation object.

func CFCopyTypeIDDescription(CFTypeID) -> CFString!

Returns a textual description of a Core Foundation type, as identified by its type ID, which can be used when debugging.

func CFShow(CFTypeRef!)

Prints a description of a Core Foundation object to stderr.

