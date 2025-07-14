

- Core Foundation
-  CFStringAppendFormatAndArguments(\_:\_:\_:\_:) 

Function

# CFStringAppendFormatAndArguments(\_:\_:\_:\_:)

Appends a formatted string to the character contents of a CFMutableString object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringAppendFormatAndArguments(
    _ theString: CFMutableString!,
    _ formatOptions: CFDictionary!,
    _ format: CFString!,
    _ arguments: CVaListPointer
)
```

## Parameters 

`theString`  

The string to which the formatted characters from `format` are appended. If this value is not a CFMutableString object, an assertion is raised.

`formatOptions`  

A dictionary containing formatting options for the string (such as the thousand-separator character, which is dependent on locale). Currently, these options are an unimplemented feature.

`format`  

A formatted string with `printf`-style specifiers.

`arguments`  

List of values to be inserted in `format`.

## Discussion

A formatted string is one with `printf`-style format specifiers embedded in the text such as `%d` (decimal), `%f` (double), and `%@` (Core Foundation object). The subsequent arguments, in order, are substituted for the specifiers in the character data appended to `theString`. You can also reorder the arguments in the string by using modifiers of the form “n\$” with the format specifiers (for example, `%2$d`).

For more information on supported specifiers, see the relevant section in String Programming Guide for Core Foundation.

## See Also

### CFMutableString Miscellaneous Functions

func CFStringAppend(CFMutableString!, CFString!)

Appends the characters of a string to those of a CFMutableString object.

func CFStringAppendCharacters(CFMutableString!, UnsafePointer&lt;UniChar>!, CFIndex)

Appends a buffer of Unicode characters to the character contents of a CFMutableString object.

func CFStringAppendCString(CFMutableString!, UnsafePointer&lt;CChar>!, CFStringEncoding)

Appends a C string to the character contents of a CFMutableString object.

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

func CFStringPad(CFMutableString!, CFString!, CFIndex, CFIndex)

Enlarges a string, padding it with specified characters, or truncates the string.

