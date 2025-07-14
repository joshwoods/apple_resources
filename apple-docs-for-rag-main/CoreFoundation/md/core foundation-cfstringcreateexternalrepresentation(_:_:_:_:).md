

- Core Foundation
-  CFStringCreateExternalRepresentation(\_:\_:\_:\_:) 

Function

# CFStringCreateExternalRepresentation(\_:\_:\_:\_:)

Creates an “external representation” of a CFString object, that is, a CFData object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringCreateExternalRepresentation(
    _ alloc: CFAllocator!,
    _ theString: CFString!,
    _ encoding: CFStringEncoding,
    _ lossByte: UInt8
) -> CFData!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new CFData object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theString`  

The string to convert to an external representation.

`encoding`  

The string encoding to use for the external representation.

`lossByte`  

The character value to assign to characters that cannot be converted to the requested encoding. Pass `0` if you want conversion to stop at the first such error; if this happens, the function returns `NULL`.

## Return Value

A CFData object that stores the characters of the CFString object as an “external representation.” Returns `NULL` if no loss byte was specified and the function could not convert the characters to the specified encoding. Ownership follows the The Create Rule.

## Discussion

In the CFData object form, the string can be written to disk as a file or be sent out over a network. If the encoding of the characters in the data object is Unicode, the function may insert a BOM (byte-order marker) to indicate endianness. However, representations created with encoding constants `kCFStringEncodingUTF16BE`, `kCFStringEncodingUTF16LE`, `kCFStringEncodingUTF32BE`, and `kCFStringEncodingUTF32LE` do not include a BOM because the byte order is explicitly indicated by the letters “BE” (big-endian) and “LE” (little-endian).

This function allows the specification of a “loss byte” to represent characters that cannot be converted to the requested encoding.

When you create an external representation from a CFMutableString object, it loses this mutability characteristic when it is converted back to a CFString object.

The CFStringCreateFromExternalRepresentation(_:_:_:) function complements this function by creating a CFString object from an “external representation” CFData object.

## See Also

### Accessing Characters

func CFStringGetBytes(CFString!, CFRange, CFStringEncoding, UInt8, Bool, UnsafeMutablePointer&lt;UInt8>!, CFIndex, UnsafeMutablePointer&lt;CFIndex>!) -> CFIndex

Fetches a range of the characters from a string into a byte buffer after converting the characters to a specified encoding.

func CFStringGetCharacterAtIndex(CFString!, CFIndex) -> UniChar

Returns the Unicode character at a specified location in a string.

func CFStringGetCharacters(CFString!, CFRange, UnsafeMutablePointer&lt;UniChar>!)

Copies a range of the Unicode characters from a string to a user-provided buffer.

func CFStringGetCharactersPtr(CFString!) -> UnsafePointer&lt;UniChar>!

Quickly obtains a pointer to the contents of a string as a buffer of Unicode characters.

func CFStringGetCharacterFromInlineBuffer(UnsafeMutablePointer&lt;CFStringInlineBuffer>!, CFIndex) -> UniChar

Returns the Unicode character at a specific location in an in-line buffer.

func CFStringGetCString(CFString!, UnsafeMutablePointer&lt;CChar>!, CFIndex, CFStringEncoding) -> Bool

Copies the character contents of a string to a local C string buffer after converting the characters to a given encoding.

func CFStringGetCStringPtr(CFString!, CFStringEncoding) -> UnsafePointer&lt;CChar>!

Quickly obtains a pointer to a C-string buffer containing the characters of a string in a given encoding.

func CFStringGetLength(CFString!) -> CFIndex

Returns the number (in terms of UTF-16 code pairs) of Unicode characters in a string.

func CFStringGetPascalString(CFString!, StringPtr!, CFIndex, CFStringEncoding) -> Bool

Copies the character contents of a CFString object to a local Pascal string buffer after converting the characters to a requested encoding.

func CFStringGetPascalStringPtr(CFString!, CFStringEncoding) -> ConstStringPtr!

Quickly obtains a pointer to a Pascal buffer containing the characters of a string in a given encoding.

func CFStringGetRangeOfComposedCharactersAtIndex(CFString!, CFIndex) -> CFRange

Returns the range of the composed character sequence at a specified index.

func CFStringInitInlineBuffer(CFString!, UnsafeMutablePointer&lt;CFStringInlineBuffer>!, CFRange)

Initializes an in-line buffer to use for efficient access of a CFString object’s characters.

