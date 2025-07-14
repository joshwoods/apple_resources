

- Core Foundation
-  CFStringCreateArrayBySeparatingStrings(\_:\_:\_:) 

Function

# CFStringCreateArrayBySeparatingStrings(\_:\_:\_:)

Creates an array of CFString objects from a single CFString object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringCreateArrayBySeparatingStrings(
    _ alloc: CFAllocator!,
    _ theString: CFString!,
    _ separatorString: CFString!
) -> CFArray!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new CFArray object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theString`  

The string to be divided into substrings. The substrings should be separated by `separatorString`.

`separatorString`  

The string used to separate the substrings in `theString`.

## Return Value

A new array that contains CFString objects that represent substrings of `theString`, or `NULL` if there was a problem creating the object. The order of elements in the array is identical to the order of the substrings in `theString`. If `separatorString` does not occur in `theString`, the result is an array containing `theString`. If `separatorString` is equal to `theString`, then the result is an array containing two empty strings. Ownership follows the The Create Rule.

## Discussion

This function provides a convenient way to convert units of data captured in a single string to a form (an array) suitable for iterative processing. One or more delimiter characters (or “separator string”) separates the substrings in the source string—these characters are frequently whitespace characters such as tabs and newlines (carriage returns). For example, you might have a file containing a localized list of place names with each name separated by a tab character. You could create a CFString object from this file and call this function on the string to obtain a CFArray object whose elements are these place names.

`separatorString` is treated as a complete unit. If you specify `XYZ` as the separator string, then if `theString` is `aXbYZcXYZe`, then the returned array contains `aXbYZc` and `e`.

See also CFStringCreateByCombiningStrings(_:_:_:).

## See Also

### Creating a CFString

func CFStringCreateByCombiningStrings(CFAllocator!, CFArray!, CFString!) -> CFString!

Creates a single string from the individual CFString objects that comprise the elements of an array.

func CFStringCreateCopy(CFAllocator!, CFString!) -> CFString!

Creates an immutable copy of a string.

func CFStringCreateFromExternalRepresentation(CFAllocator!, CFData!, CFStringEncoding) -> CFString!

Creates a string from its “external representation.”

func CFStringCreateWithBytes(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFStringEncoding, Bool) -> CFString!

Creates a string from a buffer containing characters in a specified encoding.

func CFStringCreateWithBytesNoCopy(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFStringEncoding, Bool, CFAllocator!) -> CFString!

Creates a string from a buffer, containing characters in a specified encoding, that might serve as the backing store for the new string.

func CFStringCreateWithCharacters(CFAllocator!, UnsafePointer&lt;UniChar>!, CFIndex) -> CFString!

Creates a string from a buffer of Unicode characters.

func CFStringCreateWithCharactersNoCopy(CFAllocator!, UnsafePointer&lt;UniChar>!, CFIndex, CFAllocator!) -> CFString!

Creates a string from a buffer of Unicode characters that might serve as the backing store for the object.

func CFStringCreateWithCString(CFAllocator!, UnsafePointer&lt;CChar>!, CFStringEncoding) -> CFString!

Creates an immutable string from a C string.

func CFStringCreateWithCStringNoCopy(CFAllocator!, UnsafePointer&lt;CChar>!, CFStringEncoding, CFAllocator!) -> CFString!

Creates a CFString object from an external C string buffer that might serve as the backing store for the object.

func CFStringCreateWithFormatAndArguments(CFAllocator!, CFDictionary!, CFString!, CVaListPointer) -> CFString!

Creates an immutable string from a formatted string and a variable number of arguments (specified in a parameter of type `va_list`).

func CFStringCreateWithPascalString(CFAllocator!, ConstStr255Param!, CFStringEncoding) -> CFString!

Creates an immutable CFString object from a Pascal string.

func CFStringCreateWithPascalStringNoCopy(CFAllocator!, ConstStr255Param!, CFStringEncoding, CFAllocator!) -> CFString!

Creates a CFString object from an external Pascal string buffer that might serve as the backing store for the object.

func CFStringCreateWithSubstring(CFAllocator!, CFString!, CFRange) -> CFString!

Creates an immutable string from a segment (substring) of an existing string.

