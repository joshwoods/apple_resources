

- Foundation
- NSString
-  rangeOfCharacter(from:options:range:) 

Instance Method

# rangeOfCharacter(from:options:range:)

Finds and returns the range in the string of the first character from a given character set found in a given range with given options.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func rangeOfCharacter(
    from searchSet: CharacterSet,
    options mask: NSString.CompareOptions = [],
    range rangeOfReceiverToSearch: NSRange
) -> NSRange
```

## Parameters 

`searchSet`  

A character set. This value must not be `nil`.

Raises an `NSInvalidArgumentException` if `aSet` is `nil`.

`mask`  

A mask specifying search options. The following options may be specified by combining them with the C bitwise `OR` operator: anchored, backwards.

`rangeOfReceiverToSearch`  

The range in which to search. `aRange` must not exceed the bounds of the receiver.

Raises an rangeException if `aRange` is invalid.

## Return Value

The range in the receiver of the first character found from `aSet` within `aRange`. Returns a range of ``` {``NSNotFound``, 0} ``` if none of the characters in `aSet` are found.

## Discussion

This method does not perform any Unicode normalization on the receiver, so canonically equivalent forms will not be matched. For example, searching the string “strüdel”—containing the decomposed characters “`u`” (`U+0075 LATIN SMALL LETTER U`) and “`¨`” (`U+0308 COMBINING DIAERESIS`)—with a character set containing the precomposed character “`ü`” (`U+00FC LATIN SMALL LETTER U WITH DIAERESIS`) would return the range ``` {``NSNotFound``, 0} ```, because none of the characters in the set are found.

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

func enumerateLines((String, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the lines in the string.

func enumerateSubstrings(in: NSRange, options: NSString.EnumerationOptions, using: (String?, NSRange, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates the substrings of the specified type in the specified range of the string.

