

- Core Foundation
-  CFMutableString 

Class

# CFMutableString

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFMutableString
```

## Overview

CFMutableString manages dynamic strings. The basic interface for managing strings is provided by CFString. CFMutableString adds functions to modify the contents of a string.

CFMutableString is “toll-free bridged” with its Cocoa Foundation counterpart, NSMutableString. This means that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. Therefore, in a method where you see an `NSMutableString *` parameter, you can pass in a `CFMutableStringRef`, and in a function where you see a `CFMutableStringRef` parameter, you can pass in an NSMutableString instance. This also applies to concrete subclasses of NSMutableString. See Toll-Free Bridged Types for more information on toll-free bridging.

## Topics

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

func CFStringPad(CFMutableString!, CFString!, CFIndex, CFIndex)

Enlarges a string, padding it with specified characters, or truncates the string.

func CFStringReplace(CFMutableString!, CFRange, CFString!)

Replaces part of the character contents of a CFMutableString object with another string.

func CFStringReplaceAll(CFMutableString!, CFString!)

Replaces all characters of a CFMutableString object with other characters.

func CFStringSetExternalCharactersNoCopy(CFMutableString!, UnsafeMutablePointer&lt;UniChar>!, CFIndex, CFIndex)

Notifies a CFMutableString object that its external backing store of Unicode characters has changed.

func CFStringTransform(CFMutableString!, UnsafeMutablePointer&lt;CFRange>!, CFString!, Bool) -> Bool

Perform in-place transliteration on a mutable string.

func CFStringTrim(CFMutableString!, CFString!)

Trims a specified substring from the beginning and end of a CFMutableString object.

func CFStringTrimWhitespace(CFMutableString!)

Trims whitespace from the beginning and end of a CFMutableString object.

func CFStringUppercase(CFMutableString!, CFLocale!)

Changes all lowercase alphabetical characters in a CFMutableString object to uppercase.

### Constants

enum CFStringNormalizationForm

Unicode normalization forms as described in Unicode Technical Report \#15.

Transform Identifiers for CFStringTransform

Constants that identify transforms used with CFStringTransform(_:_:_:_:).

## Relationships

### Inherits From

- CFString

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Property List Programming Topics for Core Foundation

String Programming Guide for Core Foundation

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

