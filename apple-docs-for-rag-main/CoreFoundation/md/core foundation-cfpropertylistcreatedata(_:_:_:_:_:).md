

- Core Foundation
-  CFPropertyListCreateData(\_:\_:\_:\_:\_:) 

Function

# CFPropertyListCreateData(\_:\_:\_:\_:\_:)

Returns a CFData object containing a serialized representation of a given property list in a specified format.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFPropertyListCreateData(
    _ allocator: CFAllocator!,
    _ propertyList: CFPropertyList!,
    _ format: CFPropertyListFormat,
    _ options: CFOptionFlags,
    _ error: UnsafeMutablePointer?>!
) -> Unmanaged!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new data object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`propertyList`  

The property list to write out.

`format`  

A CFPropertyListFormat constant to specify the data format. See CFPropertyListFormat for possible values.

`options`  

This parameter is currently unused and should be set to `0`.

`error`  

If this parameter is non-NULL, if an error occurs, on return this will contain a CFError error describing the problem. Ownership follows the The Create Rule.

## Return Value

A CFData object containing a serialized representation of `propertyList` in a the format specified by `format`. Ownership follows the The Create Rule.

## Discussion

## See Also

### Exporting a Property List

func CFPropertyListWrite(CFPropertyList!, CFWriteStream!, CFPropertyListFormat, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> CFIndex

Write the bytes of a serialized property list out to a stream.

func CFPropertyListCreateXMLData(CFAllocator!, CFPropertyList!) -> Unmanaged&lt;CFData>!

Creates an XML representation of the specified property list.

Deprecated

func CFPropertyListWriteToStream(CFPropertyList!, CFWriteStream!, CFPropertyListFormat, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> CFIndex

Writes the bytes of a property list serialization out to a stream.

Deprecated

