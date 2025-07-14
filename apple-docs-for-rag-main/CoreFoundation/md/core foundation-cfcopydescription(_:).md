

- Core Foundation
-  CFCopyDescription(\_:) 

Function

# CFCopyDescription(\_:)

Returns a textual description of a Core Foundation object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCopyDescription(_ cf: CFTypeRef!) -> CFString!
```

## Parameters 

`cf`  

The CFType object (a generic reference of type CFTypeRef) from which to derive a description.

## Return Value

A string that contains a description of `cf`. Ownership follows the The Create Rule.

## Discussion

The nature of the description differs by object. For example, a description of a CFArray object would include descriptions of each of the elements in the collection.

You can use this function for debugging Core Foundation objects in your code. Note, however, that the description for a given object may be different in different releases of the operating system. Do *not* create dependencies in your code on the content or format of the information returned by this function.

## See Also

### Miscellaneous Functions

func CFCopyTypeIDDescription(CFTypeID) -> CFString!

Returns a textual description of a Core Foundation type, as identified by its type ID, which can be used when debugging.

func CFGetTypeID(CFTypeRef!) -> CFTypeID

Returns the unique identifier of an opaque type to which a Core Foundation object belongs.

func CFShow(CFTypeRef!)

Prints a description of a Core Foundation object to stderr.

