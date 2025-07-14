

- Core Foundation
-  CFPropertyListCreateXMLData(\_:\_:) Deprecated

Function

# CFPropertyListCreateXMLData(\_:\_:)

Creates an XML representation of the specified property list.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFPropertyListCreateXMLData(
    _ allocator: CFAllocator!,
    _ propertyList: CFPropertyList!
) -> Unmanaged!
```

Deprecated

Use CFPropertyListCreateData instead.

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new data object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`propertyList`  

The property list to convert. This may be any of the standard property list objects, for example a CFArray or a CFDictionary object.

## Return Value

A CFData object containing the XML data. Ownership follows the The Create Rule.

## Discussion

Warning

This function is obsolete and will be deprecated soon. Use CFPropertyListCreateData(_:_:_:_:_:) instead.

## See Also

### Exporting a Property List

func CFPropertyListCreateData(CFAllocator!, CFPropertyList!, CFPropertyListFormat, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Returns a CFData object containing a serialized representation of a given property list in a specified format.

func CFPropertyListWrite(CFPropertyList!, CFWriteStream!, CFPropertyListFormat, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> CFIndex

Write the bytes of a serialized property list out to a stream.

func CFPropertyListWriteToStream(CFPropertyList!, CFWriteStream!, CFPropertyListFormat, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> CFIndex

Writes the bytes of a property list serialization out to a stream.

Deprecated

