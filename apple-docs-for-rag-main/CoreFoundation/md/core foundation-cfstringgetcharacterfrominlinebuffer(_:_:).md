

- Core Foundation
-  CFStringGetCharacterFromInlineBuffer(\_:\_:) 

Function

# CFStringGetCharacterFromInlineBuffer(\_:\_:)

Returns the Unicode character at a specific location in an in-line buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringGetCharacterFromInlineBuffer(
    _ buf: UnsafeMutablePointer!,
    _ idx: CFIndex
) -> UniChar
```

## Parameters 

`buf`  

The initialized CFStringInlineBuffer structure in which the characters are stored. You should initialize the structure with the CFStringInitInlineBuffer(_:_:_:) function.

`idx`  

The location of a character in the in-line buffer `buf`. This index is relative to the range specified when `buf` was created.

## Return Value

A Unicode character, or `0` if a location outside the original range is specified.

## Discussion

This function accesses one of the characters of a string written to an in-line buffer. It is typically called from within a loop to access each character in the buffer in sequence. You should initialize the buffer with the CFStringInitInlineBuffer(_:_:_:) function. The in-line buffer functions, along with the CFStringInlineBuffer structure, give you fast access to the characters of a CFString object. The technique for in-line buffer access combines the convenience of one-at-a-time character access with the efficiency of bulk access.

## See Also

### Accessing Characters

func CFStringCreateExternalRepresentation(CFAllocator!, CFString!, CFStringEncoding, UInt8) -> CFData!

Creates an “external representation” of a CFString object, that is, a CFData object.

func CFStringGetBytes(CFString!, CFRange, CFStringEncoding, UInt8, Bool, UnsafeMutablePointer&lt;UInt8>!, CFIndex, UnsafeMutablePointer&lt;CFIndex>!) -> CFIndex

Fetches a range of the characters from a string into a byte buffer after converting the characters to a specified encoding.

func CFStringGetCharacterAtIndex(CFString!, CFIndex) -> UniChar

Returns the Unicode character at a specified location in a string.

func CFStringGetCharacters(CFString!, CFRange, UnsafeMutablePointer&lt;UniChar>!)

Copies a range of the Unicode characters from a string to a user-provided buffer.

func CFStringGetCharactersPtr(CFString!) -> UnsafePointer&lt;UniChar>!

Quickly obtains a pointer to the contents of a string as a buffer of Unicode characters.

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

