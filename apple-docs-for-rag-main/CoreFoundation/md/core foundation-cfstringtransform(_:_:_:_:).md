

- Core Foundation
-  CFStringTransform(\_:\_:\_:\_:) 

Function

# CFStringTransform(\_:\_:\_:\_:)

Perform in-place transliteration on a mutable string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringTransform(
    _ string: CFMutableString!,
    _ range: UnsafeMutablePointer!,
    _ transform: CFString!,
    _ reverse: Bool
) -> Bool
```

## Parameters 

`string`  

The string to transform.

`range`  

A pointer to the range over which the transformation is applied. `NULL` causes the whole string to be transformed. On return, `range` is modified to reflect the new range corresponding to the original range.

`transform`  

A CFString object that identifies the transformation to apply. For a list of valid values, see Transform Identifiers for CFStringTransform. In macOS 10.4 and later, you can also use any valid ICU transform ID defined in the ICU User Guide for Transforms.

`reverse`  

A Boolean that, if `true`, specifies that the inverse transform should be used (if it exists).

## Return Value

`true` if the transform is successful; otherwise `false`.

## Discussion

The transformation represented by `transform` is applied to the given range of `string`, modifying it in place. Only the specified range is modified, but the transform may look at portions of the string outside that range for context. Reasons that the transform may be unsuccessful include an invalid transform identifier, and attempting to reverse an irreversible transform.

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

