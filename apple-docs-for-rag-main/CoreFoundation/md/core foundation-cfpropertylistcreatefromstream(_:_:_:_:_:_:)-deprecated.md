

- Core Foundation
-  CFPropertyListCreateFromStream(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# CFPropertyListCreateFromStream(\_:\_:\_:\_:\_:\_:)

Creates a property list using data from a stream.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFPropertyListCreateFromStream(
    _ allocator: CFAllocator!,
    _ stream: CFReadStream!,
    _ streamLength: CFIndex,
    _ mutabilityOption: CFOptionFlags,
    _ format: UnsafeMutablePointer!,
    _ errorString: UnsafeMutablePointer?>!
) -> Unmanaged!
```

Deprecated

Use CFPropertyListCreateWithStream instead.

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new property list. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`stream`  

The stream whose data contains the content. The stream must be opened and configured—this function simply reads bytes from the stream. The stream may contain any supported property list type (see CFPropertyListFormat).

`streamLength`  

The number of bytes to read. If `0`, this function will read to the end of the stream.

`mutabilityOption`  

A constant that specifies the degree of mutability for the returned property list. See Property List Mutability Options for descriptions of possible values.

`format`  

A constant that specifies the format of the property list. See CFPropertyListFormat for possible values.

`errorString`  

On return, `NULL` if the conversion is successful, otherwise a string that describes the nature of the error. Error messages are not localized, but may be in the future, so they are not suitable for comparison.

Pass `NULL` if you do not wish to receive an error string. Ownership follows the The Create Rule.

## Return Value

A new property list initialized with the data contained in `stream`. Ownership follows the The Create Rule.

## Discussion

This function simply reads bytes from `stream` starting at the current location to the end, which is expected to be the end of the property list, or up to the number of bytes specified by `streamLength` if it is not `0`.

### Special Considerations

Warning

This function is obsolete and will be deprecated soon. Use CFPropertyListCreateWithStream(_:_:_:_:_:_:) instead.

## See Also

### Creating a Property List

func CFPropertyListCreateWithData(CFAllocator!, CFData!, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list from a given CFData object.

func CFPropertyListCreateWithStream(CFAllocator!, CFReadStream!, CFIndex, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFPropertyList>!

Create and return a property list with a CFReadStream input.

func CFPropertyListCreateDeepCopy(CFAllocator!, CFPropertyList!, CFOptionFlags) -> CFPropertyList!

Recursively creates a copy of a given property list.

func CFPropertyListCreateFromXMLData(CFAllocator!, CFData!, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list using the specified XML or binary property list data.

Deprecated

