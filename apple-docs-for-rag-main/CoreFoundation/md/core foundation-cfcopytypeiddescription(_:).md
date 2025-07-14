

- Core Foundation
-  CFCopyTypeIDDescription(\_:) 

Function

# CFCopyTypeIDDescription(\_:)

Returns a textual description of a Core Foundation type, as identified by its type ID, which can be used when debugging.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCopyTypeIDDescription(_ type_id: CFTypeID) -> CFString!
```

## Parameters 

`type_id`  

An integer of type CFTypeID that uniquely identifies a Core Foundation opaque type.

## Return Value

A string containing a type description. Ownership follows the The Create Rule.

## Discussion

You can use this function for debugging Core Foundation objects in your code. Note, however, that the description for a given object may be different in different releases of the operating system. Do *not* create dependencies in your code on the content or format of the information returned by this function.

## See Also

### Miscellaneous Functions

func CFCopyDescription(CFTypeRef!) -> CFString!

Returns a textual description of a Core Foundation object.

func CFGetTypeID(CFTypeRef!) -> CFTypeID

Returns the unique identifier of an opaque type to which a Core Foundation object belongs.

func CFShow(CFTypeRef!)

Prints a description of a Core Foundation object to stderr.

