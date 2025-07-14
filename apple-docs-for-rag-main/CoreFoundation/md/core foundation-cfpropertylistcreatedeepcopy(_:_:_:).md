

- Core Foundation
-  CFPropertyListCreateDeepCopy(\_:\_:\_:) 

Function

# CFPropertyListCreateDeepCopy(\_:\_:\_:)

Recursively creates a copy of a given property list.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPropertyListCreateDeepCopy(
    _ allocator: CFAllocator!,
    _ propertyList: CFPropertyList!,
    _ mutabilityOption: CFOptionFlags
) -> CFPropertyList!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new property list. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`propertyList`  

The property list to copy. This may be any of the standard property list objects, for example a CFArray or a CFDictionary object.

`mutabilityOption`  

A constant that specifies the degree of mutability of the returned property list. See Property List Mutability Options for descriptions of possible values.

## Return Value

A new property list that is a copy of `propertyList`. Ownership follows the The Create Rule.

## Discussion

Recursively creates a copy of the given property list so nested arrays and dictionaries are copied as well as the top-most container.

## See Also

### Creating a Property List

func CFPropertyListCreateWithData(CFAllocator!, CFData!, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list from a given CFData object.

func CFPropertyListCreateWithStream(CFAllocator!, CFReadStream!, CFIndex, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFPropertyList>!

Create and return a property list with a CFReadStream input.

func CFPropertyListCreateFromXMLData(CFAllocator!, CFData!, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list using the specified XML or binary property list data.

Deprecated

func CFPropertyListCreateFromStream(CFAllocator!, CFReadStream!, CFIndex, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list using data from a stream.

Deprecated

