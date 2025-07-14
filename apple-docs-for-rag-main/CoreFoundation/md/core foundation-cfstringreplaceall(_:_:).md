

- Core Foundation
-  CFStringReplaceAll(\_:\_:) 

Function

# CFStringReplaceAll(\_:\_:)

Replaces all characters of a CFMutableString object with other characters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringReplaceAll(
    _ theString: CFMutableString!,
    _ replacement: CFString!
)
```

## Parameters 

`theString`  

The string to modify. If this value is not a CFMutableString object, an assertion is raised.

`replacement`  

The replacement string to put into `theString`.

## Discussion

The character buffer of `theString` is resized according to the length of the new characters.

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

func CFStringCreateMutableCopy(CFAllocator!, CFIndex, CFString!) -> CFMutableString!

Creates a mutable copy of a string.

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

