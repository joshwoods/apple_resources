

- Core Foundation
-  CFStringPad(\_:\_:\_:\_:) 

Function

# CFStringPad(\_:\_:\_:\_:)

Enlarges a string, padding it with specified characters, or truncates the string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringPad(
    _ theString: CFMutableString!,
    _ padString: CFString!,
    _ length: CFIndex,
    _ indexIntoPad: CFIndex
)
```

## Parameters 

`theString`  

The string to modify.

`padString`  

A string containing the characters with which to fill the extended character buffer. Pass `NULL` to truncate the string.

`length`  

The new length of `theString`. If this length is greater than the current length, padding takes place; if it is less, truncation takes place.

`indexIntoPad`  

The index of the character in `padString` with which to begin padding. If you are truncating the string represented by the object, this parameter is ignored.

## Discussion

This function has two purposes. It either enlarges the character buffer of a CFMutableString object to a given length, padding the added length with a given character or characters, or it truncates the character buffer to a smaller size. The key parameter for this behavior is `length`; if it is greater than the current length of the represented string, padding takes place, and if it less than the current length, truncation occurs.

For example, say you have a string, `aMutStr`, containing the characters “abcdef”. The call

```
CFStringPad(aMutStr, CFSTR("123"), 9, 1);
```

results in `aMutStr` containing “abcdef231”. However, the following call

```
CFStringPad(aMutStr, NULL, 3, 0);
```

results in `aMutStr` containing “abc”.

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

