

- Core Foundation
-  CFStringReplace(\_:\_:\_:) 

Function

# CFStringReplace(\_:\_:\_:)

Replaces part of the character contents of a CFMutableString object with another string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringReplace(
    _ theString: CFMutableString!,
    _ range: CFRange,
    _ replacement: CFString!
)
```

## Parameters 

`theString`  

The string to modify. The characters are adjusted left or right (depending on the length of the substituted string) and the character buffer of the object is resized accordingly. If this value is not a CFMutableString object, an assertion is raised.

`range`  

The range of characters in `theString` to replace.

`replacement`  

The replacement string to put into `theString`.

## Discussion

Although you can use this function to replace all characters in a CFMutableString object (by specifying a range of `(0, CFStringGetLength(theString))` ), it is more convenient to use the CFStringReplaceAll(_:_:) function for that purpose.

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

