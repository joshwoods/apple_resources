

- Foundation
- NSString
-  rangeOfCharacter(from:options:) 

Instance Method

# rangeOfCharacter(from:options:)

Finds and returns the range in the string of the first character, using given options, from a given character set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func rangeOfCharacter(
    from searchSet: CharacterSet,
    options mask: NSString.CompareOptions = []
) -> NSRange
```

## Parameters 

`searchSet`  

A character set. This value must not be `nil`.

Raises an `NSInvalidArgumentException` if `aSet` is `nil`.

`mask`  

A mask specifying search options. The following options may be specified by combining them with the C bitwise `OR` operator: anchored, backwards.

## Return Value

The range in the receiver of the first character found from `aSet`. Returns a range of ``` {``NSNotFound``, 0} ``` if none of the characters in `aSet` are found.

## Discussion

Invokes rangeOfCharacter(from:options:range:) with `mask` for the options and the entire extent of the receiver for the range.

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

func enumerateLines((String, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the lines in the string.

func enumerateSubstrings(in: NSRange, options: NSString.EnumerationOptions, using: (String?, NSRange, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates the substrings of the specified type in the specified range of the string.

