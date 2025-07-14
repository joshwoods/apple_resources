

- Core Foundation
-  CFPropertyListCreateFromXMLData(\_:\_:\_:\_:) Deprecated

Function

# CFPropertyListCreateFromXMLData(\_:\_:\_:\_:)

Creates a property list using the specified XML or binary property list data.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFPropertyListCreateFromXMLData(
    _ allocator: CFAllocator!,
    _ xmlData: CFData!,
    _ mutabilityOption: CFOptionFlags,
    _ errorString: UnsafeMutablePointer?>!
) -> Unmanaged!
```

Deprecated

Use CFPropertyListCreateWithData instead.

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new property list. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`xmlData`  

The raw bytes to convert into a property list. The bytes may be the content of an XML file or of a binary property list (see CFPropertyListFormat).

`mutabilityOption`  

A constant that specifies the degree of mutability for the returned property list. See Property List Mutability Options for descriptions of possible values.

`errorString`  

On return, `NULL` if the conversion is successful, otherwise a string that describes the nature of the error. Error messages are not localized, but may be in the future, so they are not currently suitable for comparison.

Pass `NULL` if you do not wish to receive an error string. Ownership follows the The Create Rule.

## Return Value

A new property list if the conversion is successful, otherwise `NULL`. Ownership follows the The Create Rule.

## Discussion

Warning

This function is obsolete and will be deprecated soon. Use CFPropertyListCreateWithData(_:_:_:_:_:) instead.

## See Also

### Creating a Property List

func CFPropertyListCreateWithData(CFAllocator!, CFData!, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list from a given CFData object.

func CFPropertyListCreateWithStream(CFAllocator!, CFReadStream!, CFIndex, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFPropertyList>!

Create and return a property list with a CFReadStream input.

func CFPropertyListCreateDeepCopy(CFAllocator!, CFPropertyList!, CFOptionFlags) -> CFPropertyList!

Recursively creates a copy of a given property list.

func CFPropertyListCreateFromStream(CFAllocator!, CFReadStream!, CFIndex, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list using data from a stream.

Deprecated

