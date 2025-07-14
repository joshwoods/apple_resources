

- Core Foundation
-  CFStringCreateMutableCopy(\_:\_:\_:) 

Function

# CFStringCreateMutableCopy(\_:\_:\_:)

Creates a mutable copy of a string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringCreateMutableCopy(
    _ alloc: CFAllocator!,
    _ maxLength: CFIndex,
    _ theString: CFString!
) -> CFMutableString!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new string. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`maxLength`  

The maximum number of Unicode characters that can be stored by the returned object. Pass `0` if there should be no character limit. Note that initially the returned object still has the same length as the string argument; this parameter simply specifies what the maximum size is. CFString might try to optimize its internal storage by paying attention to this value.

`theString`  

A string to copy.

## Return Value

A string that has the same contents as `theString`. Returns `NULL` if there was a problem copying the object. Ownership follows the The Create Rule.

## Discussion

The returned mutable string is identical to the original string except for (perhaps) the mutability attribute. You can add character data to the returned string with any of the `CFStringAppend...` functions, and you can insert, delete, replace, pad, and trim characters with the appropriate CFString functions. If the `maxLength` parameter is greater than `0`, any attempt to add characters beyond this limit results in a run-time error.

## See Also

### CFMutableString Miscellaneous Functions

func CFStringAppend(CFMutableString!, CFString!)

Appends the characters of a string to those of a CFMutableString object.

func CFStringAppendCharacters(CFMutableString!, UnsafePointer&lt;UniChar>!, CFIndex)

Appends a buffer of Unicode characters to the character contents of a CFMutableString object.

func CFStringAppendCString(CFMutableString!, UnsafePointer&lt;CChar>!, CFStringEncoding)

Appends a C string to the character contents of a CFMutableString object.

func CFStringAppendFormatAndArguments(CFMutableString!, CFDictionary!, CFString!, CVaListPointer)

Appends a formatted string to the character contents of a CFMutableString object.

func CFStringAppendPascalString(CFMutableString!, ConstStr255Param!, CFStringEncoding)

Appends a Pascal string to the character contents of a CFMutableString object.

func CFStringCapitalize(CFMutableString!, CFLocale!)

Changes the first character in each word of a string to uppercase (if it is a lowercase alphabetical character).

func CFStringCreateMutable(CFAllocator!, CFIndex) -> CFMutableString!

Creates an empty CFMutableString object.

func CFStringCreateMutableWithExternalCharactersNoCopy(CFAllocator!, UnsafeMutablePointer&lt;UniChar>!, CFIndex, CFIndex, CFAllocator!) -> CFMutableString!

Creates a CFMutableString object whose Unicode character buffer is controlled externally.

func CFStringDelete(CFMutableString!, CFRange)

Deletes a range of characters in a string.

func CFStringFindAndReplace(CFMutableString!, CFString!, CFString!, CFRange, CFStringCompareFlags) -> CFIndex

Replaces all occurrences of a substring within a given range.

func CFStringFold(CFMutableString!, CFStringCompareFlags, CFLocale!)

Folds a given string into the form specified by optional flags.

func CFStringInsert(CFMutableString!, CFIndex, CFString!)

Inserts a string at a specified location in the character buffer of a CFMutableString object.

func CFStringLowercase(CFMutableString!, CFLocale!)

Changes all uppercase alphabetical characters in a CFMutableString to lowercase.

func CFStringNormalize(CFMutableString!, CFStringNormalizationForm)

Normalizes the string into the specified form as described in Unicode Technical Report \#15.

func CFStringPad(CFMutableString!, CFString!, CFIndex, CFIndex)

Enlarges a string, padding it with specified characters, or truncates the string.

