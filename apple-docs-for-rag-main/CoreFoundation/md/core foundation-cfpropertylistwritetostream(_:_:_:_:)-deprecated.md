

- Core Foundation
-  CFPropertyListWriteToStream(\_:\_:\_:\_:) Deprecated

Function

# CFPropertyListWriteToStream(\_:\_:\_:\_:)

Writes the bytes of a property list serialization out to a stream.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFPropertyListWriteToStream(
    _ propertyList: CFPropertyList!,
    _ stream: CFWriteStream!,
    _ format: CFPropertyListFormat,
    _ errorString: UnsafeMutablePointer?>!
) -> CFIndex
```

Deprecated

Use CFPropertyListWrite instead.

## Parameters 

`propertyList`  

The property list to write out.

`stream`  

The stream to write to. The stream must be opened and configured—this function simply writes bytes to the stream.

`format`  

A constant that specifies the format used to write `propertyList`. See CFPropertyListFormat for possible values.

`errorString`  

On return, `NULL` if the conversion is successful, otherwise a string that describes the nature of the errors. Error messages are not localized, but may be in the future, so they are not currently suitable for comparison.

Pass `NULL` if you do not wish to receive an error string. Ownership follows the The Create Rule.

## Return Value

The number of bytes written, or `0` if an error occurred. If `0` is returned, `errorString` will contain an error message.

## Discussion

This function leaves the stream open after reading the content. When reading a property list, this function expects the reading stream to end wherever the writing ended, so that the end of the property list data can be identified.

### Special Considerations

Warning

This function is obsolete and will be deprecated soon. Use CFPropertyListWrite(_:_:_:_:_:) instead.

## See Also

### Exporting a Property List

func CFPropertyListCreateData(CFAllocator!, CFPropertyList!, CFPropertyListFormat, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Returns a CFData object containing a serialized representation of a given property list in a specified format.

func CFPropertyListWrite(CFPropertyList!, CFWriteStream!, CFPropertyListFormat, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> CFIndex

Write the bytes of a serialized property list out to a stream.

func CFPropertyListCreateXMLData(CFAllocator!, CFPropertyList!) -> Unmanaged&lt;CFData>!

Creates an XML representation of the specified property list.

Deprecated

