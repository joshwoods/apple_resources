

- Core Foundation
-  CFStringFindAndReplace(\_:\_:\_:\_:\_:) 

Function

# CFStringFindAndReplace(\_:\_:\_:\_:\_:)

Replaces all occurrences of a substring within a given range.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringFindAndReplace(
    _ theString: CFMutableString!,
    _ stringToFind: CFString!,
    _ replacementString: CFString!,
    _ rangeToSearch: CFRange,
    _ compareOptions: CFStringCompareFlags
) -> CFIndex
```

## Parameters 

`theString`  

The string to modify.

`stringToFind`  

The substring to search for in `theString`.

`replacementString`  

The replacement string for `stringToFind`.

`rangeToSearch`  

The range within which to search in `theString`.

`compareOptions`  

Flags that select different types of comparisons, such as localized comparison, case-insensitive comparison, and non-literal comparison. If you want the default comparison behavior, pass `0`. See CFStringCompareFlags for the available flags.

## Return Value

The number of instances of `stringToFind` that were replaced.

## Discussion

The possible values of `compareOptions` are combinations of the compareCaseInsensitive, compareBackwards, compareNonliteral, and compareAnchored constants.

The `kCFCompareBackwards` option can be used to replace a substring starting from the end, which could produce different results. For example, if the parameter `theString` is “AAAAA”, `stringToFind` is “AA”, and `replacementString` is “B”, then the result is normally “BBA”. However, if the `kCFCompareBackwards` constant is used, the result is “ABB.”

The `kCFCompareAnchored` option assures that only anchored but multiple instances are found (the instances must be consecutive at start or end). For example, if the parameter `theString` is “AAXAA”, `stringToFind` is “A”, and `replacementString` is “B”, then the result is normally “BBXBB.” However, if the `kCFCompareAnchored` constant is used, the result is “BBXAA.”

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

