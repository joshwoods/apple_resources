

- Core Foundation
-  CFPropertyListCreateWithStream(\_:\_:\_:\_:\_:\_:) 

Function

# CFPropertyListCreateWithStream(\_:\_:\_:\_:\_:\_:)

Create and return a property list with a CFReadStream input.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFPropertyListCreateWithStream(
    _ allocator: CFAllocator!,
    _ stream: CFReadStream!,
    _ streamLength: CFIndex,
    _ options: CFOptionFlags,
    _ format: UnsafeMutablePointer!,
    _ error: UnsafeMutablePointer?>!
) -> Unmanaged!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new property list object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`stream`  

A CFReadStream that contains a serialized representation of a property list.

`streamLength`  

The number of bytes to read from the stream. Pass `0` to read until the end of the stream is detected.

`options`  

A CFPropertyListMutabilityOptions constant to specify the mutability of the returned property list—see Property List Mutability Options for possible values.

`format`  

If this parameter is non-`NULL`, on return it will be set to the format of the data. See CFPropertyListFormat for possible values.

`error`  

If this parameter is non-`NULL`, if an error occurs, on return this will contain a CFError error describing the problem. Ownership follows the The Create Rule.

## Return Value

A new property list created from the data in `stream`. If an error occurs while parsing the data, returns `NULL`. Ownership follows the The Create Rule.

## See Also

### Creating a Property List

func CFPropertyListCreateWithData(CFAllocator!, CFData!, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list from a given CFData object.

func CFPropertyListCreateDeepCopy(CFAllocator!, CFPropertyList!, CFOptionFlags) -> CFPropertyList!

Recursively creates a copy of a given property list.

func CFPropertyListCreateFromXMLData(CFAllocator!, CFData!, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list using the specified XML or binary property list data.

Deprecated

func CFPropertyListCreateFromStream(CFAllocator!, CFReadStream!, CFIndex, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list using data from a stream.

Deprecated

