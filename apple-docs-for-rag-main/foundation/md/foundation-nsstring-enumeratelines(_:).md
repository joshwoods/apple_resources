

- Foundation
- NSString
-  enumerateLines(\_:) 

Instance Method

# enumerateLines(\_:)

Enumerates all the lines in the string.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerateLines(_ block: @escaping (String, UnsafeMutablePointer) -> Void)
```

## Parameters 

`block`  

The block executed for the enumeration.

The block takes two arguments:

line  
The current line of the string being enumerated. The line contains just the contents of the line, without the line terminators. See getLineStart(_:end:contentsEnd:for:) for a discussion of line terminators.

stop  
A reference to a Boolean value that the block can use to stop the enumeration by setting `*stop = YES`; it should not touch `*stop` otherwise.

## See Also

### Finding Characters and Substrings

func contains(String) -> Bool

Returns a Boolean value indicating whether the string contains a given string by performing a case-sensitive, locale-unaware search.

func localizedCaseInsensitiveContains(String) -> Bool

Returns a Boolean value indicating whether the string contains a given string by performing a case-insensitive, locale-aware search.

func localizedStandardContains(String) -> Bool

Returns a Boolean value indicating whether the string contains a given string by performing a case and diacritic insensitive, locale-aware search.

func rangeOfCharacter(from: CharacterSet) -> NSRange

Finds and returns the range in the string of the first character from a given character set.

func rangeOfCharacter(from: CharacterSet, options: NSString.CompareOptions) -> NSRange

Finds and returns the range in the string of the first character, using given options, from a given character set.

func rangeOfCharacter(from: CharacterSet, options: NSString.CompareOptions, range: NSRange) -> NSRange

Finds and returns the range in the string of the first character from a given character set found in a given range with given options.

func range(of: String) -> NSRange

Finds and returns the range of the first occurrence of a given string within the string.

func range(of: String, options: NSString.CompareOptions) -> NSRange

Finds and returns the range of the first occurrence of a given string within the string, subject to given options.

func range(of: String, options: NSString.CompareOptions, range: NSRange) -> NSRange

Finds and returns the range of the first occurrence of a given string, within the given range of the string, subject to given options.

func range(of: String, options: NSString.CompareOptions, range: NSRange, locale: Locale?) -> NSRange

Finds and returns the range of the first occurrence of a given string within a given range of the string, subject to given options, using the specified locale, if any.

func localizedStandardRange(of: String) -> NSRange

Finds and returns the range of the first occurrence of a given string within the string by performing a case and diacritic insensitive, locale-aware search.

func enumerateSubstrings(in: NSRange, options: NSString.EnumerationOptions, using: (String?, NSRange, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates the substrings of the specified type in the specified range of the string.

