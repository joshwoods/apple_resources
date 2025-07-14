

- Core Foundation
-  CFPropertyListWrite(\_:\_:\_:\_:\_:) 

Function

# CFPropertyListWrite(\_:\_:\_:\_:\_:)

Write the bytes of a serialized property list out to a stream.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFPropertyListWrite(
    _ propertyList: CFPropertyList!,
    _ stream: CFWriteStream!,
    _ format: CFPropertyListFormat,
    _ options: CFOptionFlags,
    _ error: UnsafeMutablePointer?>!
) -> CFIndex
```

## Parameters 

`propertyList`  

The property list to write out.

`stream`  

The CFWriteStream to which to write the data. The stream must be opened and configured.

`format`  

A CFPropertyListFormat constant to specify the data format. See CFPropertyListFormat for possible values.

`options`  

This parameter is currently unused and should be set to `0`.

`error`  

If this parameter is non-NULL, if an error occurs, on return this will contain a CFError error describing the problem. Ownership follows the The Create Rule.

## Return Value

The number of bytes written to `stream`. If an error occurs, returns `0`.

## See Also

### Exporting a Property List

func CFPropertyListCreateData(CFAllocator!, CFPropertyList!, CFPropertyListFormat, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Returns a CFData object containing a serialized representation of a given property list in a specified format.

func CFPropertyListCreateXMLData(CFAllocator!, CFPropertyList!) -> Unmanaged&lt;CFData>!

Creates an XML representation of the specified property list.

Deprecated

func CFPropertyListWriteToStream(CFPropertyList!, CFWriteStream!, CFPropertyListFormat, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> CFIndex

Writes the bytes of a property list serialization out to a stream.

Deprecated

