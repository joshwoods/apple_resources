

- Core Foundation
-  CFStringLowercase(\_:\_:) 

Function

# CFStringLowercase(\_:\_:)

Changes all uppercase alphabetical characters in a CFMutableString to lowercase.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringLowercase(
    _ theString: CFMutableString!,
    _ locale: CFLocale!
)
```

## Parameters 

`theString`  

The string to be lowercased. If this value is not a CFMutableString object, an assertion is raised.

`locale`  

The locale to use when the lowercasing operation is performed. Prior to OS X v10.3 this parameter was an untyped pointer and not used.

The locale argument affects the case mapping algorithm. For example, for the Turkish locale, case-insensitive compare matches “I” to “ı” (Unicode code point U+0131, Latin Small Dotless I), not the normal “i” character.

## Discussion

The `locale` parameter type changed from void \* to CFLocaleRef in OS X v10.3.

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

func CFStringNormalize(CFMutableString!, CFStringNormalizationForm)

Normalizes the string into the specified form as described in Unicode Technical Report \#15.

func CFStringPad(CFMutableString!, CFString!, CFIndex, CFIndex)

Enlarges a string, padding it with specified characters, or truncates the string.

