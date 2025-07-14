

- Swift
-  StringProtocol 

Protocol

# StringProtocol

A type that can represent a string as a collection of characters.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol StringProtocol : BidirectionalCollection, Comparable, ExpressibleByStringInterpolation, Hashable, LosslessStringConvertible, TextOutputStream, TextOutputStreamable where Self.Element == Character, Self.Index == String.Index, Self.StringInterpolation == DefaultStringInterpolation, Self.SubSequence : StringProtocol
```

## Overview

Do not declare new conformances to `StringProtocol`. Only the `String` and `Substring` types in the standard library are valid conforming types.

## Topics

### Operators

static func != &lt;RHS>(Self, RHS) -> Bool

### Associated Types

associatedtype SubSequence = Substring

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

**Required**

associatedtype UTF16View : BidirectionalCollection

**Required**

associatedtype UTF8View : Collection

**Required**

associatedtype UnicodeScalarView : BidirectionalCollection

**Required**

### Initializers

init(cString: UnsafePointer&lt;CChar>)

Creates a string from the null-terminated, UTF-8 encoded sequence of bytes at the given pointer.

**Required**

init&lt;C, Encoding>(decoding: C, as: Encoding.Type)

Creates a string from the given Unicode code units in the specified encoding.

**Required**

init&lt;Encoding>(decodingCString: UnsafePointer&lt;Encoding.CodeUnit>, as: Encoding.Type)

Creates a string from the null-terminated sequence of bytes at the given pointer.

**Required**

### Instance Properties

var capitalized: String

A copy of the string with each word changed to its corresponding capitalized spelling.

var decomposedStringWithCanonicalMapping: String

A string created by normalizing the string’s contents using Form D.

var decomposedStringWithCompatibilityMapping: String

A string created by normalizing the string’s contents using Form KD.

var fastestEncoding: String.Encoding

The fastest encoding to which the string can be converted without loss of information.

var hash: Int

An unsigned integer that can be used as a hash table address.

var localizedCapitalized: String

A capitalized representation of the string that is produced using the current locale.

var localizedLowercase: String

A lowercase version of the string that is produced using the current locale.

var localizedUppercase: String

An uppercase version of the string that is produced using the current locale.

var precomposedStringWithCanonicalMapping: String

A string created by normalizing the string’s contents using Form C.

var precomposedStringWithCompatibilityMapping: String

A string created by normalizing the string’s contents using Form KC.

var removingPercentEncoding: String?

A new string made from the string by replacing all percent encoded sequences with the matching UTF-8 characters.

var smallestEncoding: String.Encoding

The smallest encoding to which the string can be converted without loss of information.

var unicodeScalars: Self.UnicodeScalarView

**Required**

var utf16: Self.UTF16View

**Required**

var utf8: Self.UTF8View

**Required**

### Instance Methods

func addingPercentEncoding(withAllowedCharacters: CharacterSet) -> String?

Returns a new string created by replacing all characters in the string not in the specified set with percent encoded characters.

func addingPercentEscapes(using: String.Encoding) -> String?

Returns a representation of the `String` using a given encoding to determine the percent escapes necessary to convert the `String` into a legal URL string.

func appending(some StringProtocol) -> String

Returns a new string created by appending the given string.

func appendingFormat&lt;T>(T, any CVarArg...) -> String

Returns a string created by appending a string constructed from a given format string and the following arguments.

func applyingTransform(StringTransform, reverse: Bool) -> String?

Perform string transliteration.

func cString(using: String.Encoding) -> [CChar]?

Returns a representation of the string as a C string using a given encoding.

func canBeConverted(to: String.Encoding) -> Bool

Returns a Boolean value that indicates whether the string can be converted to the specified encoding without loss of information.

func capitalized(with: Locale?) -> String

Returns a capitalized representation of the string using the specified locale.

func caseInsensitiveCompare&lt;T>(T) -> ComparisonResult

Returns the result of invoking `compare:options:` with `NSCaseInsensitiveSearch` as the only option.

func commonPrefix&lt;T>(with: T, options: String.CompareOptions) -> String

Returns a string containing characters this string and the given string have in common, starting from the beginning of each up to the first characters that aren’t equivalent.

func compare&lt;T>(T, options: String.CompareOptions, range: Range&lt;Self.Index>?, locale: Locale?) -> ComparisonResult

Compares the string using the specified options and returns the lexical ordering for the range.

func completePath(into: UnsafeMutablePointer&lt;String>?, caseSensitive: Bool, matchesInto: UnsafeMutablePointer&lt;[String]>?, filterTypes: [String]?) -> Int

Interprets the string as a path in the file system and attempts to perform filename completion, returning a numeric value that indicates whether a match was possible, and by reference the longest path that matches the string.

func components(separatedBy: CharacterSet) -> [String]

Returns an array containing substrings from the string that have been divided by characters in the given set.

func components&lt;T>(separatedBy: T) -> [String]

Returns an array containing substrings from the string that have been divided by the given separator.

func contains&lt;T>(T) -> Bool

Returns `true` if `other` is non-empty and contained within `self` by case-sensitive, non-literal search. Otherwise, returns `false`.

func contains(String) -> Bool

func contains(Substring) -> Bool

func data(using: String.Encoding, allowLossyConversion: Bool) -> Data?

Returns a `Data` containing a representation of the `String` encoded using a given encoding.

func enumerateLines(invoking: (String, inout Bool) -> Void)

Enumerates all the lines in a string.

func enumerateLinguisticTags&lt;T, R>(in: R, scheme: T, options: NSLinguisticTagger.Options, orthography: NSOrthography?, invoking: (String, Range&lt;Self.Index>, Range&lt;Self.Index>, inout Bool) -> Void)

Performs linguistic analysis on the specified string by enumerating the specific range of the string, providing the Block with the located tags.

func enumerateSubstrings&lt;R>(in: R, options: String.EnumerationOptions, (String?, Range&lt;Self.Index>, Range&lt;Self.Index>, inout Bool) -> Void)

Enumerates the substrings of the specified type in the specified range of the string.

func folding(options: String.CompareOptions, locale: Locale?) -> String

Returns a string with the given character folding options applied.

func getBytes&lt;R>(inout [UInt8], maxLength: Int, usedLength: UnsafeMutablePointer&lt;Int>, encoding: String.Encoding, options: String.EncodingConversionOptions, range: R, remaining: UnsafeMutablePointer&lt;Range&lt;Self.Index>>) -> Bool

Writes the given `range` of characters into `buffer` in a given `encoding`, without any allocations. Does not NULL-terminate.

func getCString(inout [CChar], maxLength: Int, encoding: String.Encoding) -> Bool

Converts the `String`’s content to a given encoding and stores them in a buffer.

func getLineStart(UnsafeMutablePointer&lt;Self.Index>, end: UnsafeMutablePointer&lt;Self.Index>, contentsEnd: UnsafeMutablePointer&lt;Self.Index>, for: some RangeExpression&lt;String.Index>)

Returns by reference the beginning of the first line and the end of the last line touched by the given range.

func getParagraphStart(UnsafeMutablePointer&lt;Self.Index>, end: UnsafeMutablePointer&lt;Self.Index>, contentsEnd: UnsafeMutablePointer&lt;Self.Index>, for: some RangeExpression&lt;String.Index>)

Returns by reference the beginning of the first paragraph and the end of the last paragraph touched by the given range.

func hasPrefix(String) -> Bool

**Required** Default implementation provided.

func hasSuffix(String) -> Bool

**Required** Default implementation provided.

func lengthOfBytes(using: String.Encoding) -> Int

Returns the number of bytes required to store the `String` in a given encoding.

func lineRange(for: some RangeExpression&lt;String.Index>) -> Range&lt;Self.Index>

Returns the range of characters representing the line or lines containing a given range.

func linguisticTags&lt;T, R>(in: R, scheme: T, options: NSLinguisticTagger.Options, orthography: NSOrthography?, tokenRanges: UnsafeMutablePointer&lt;[Range&lt;Self.Index>]>?) -> [String]

Returns an array of linguistic tags for the specified range and requested tags within the receiving string.

func localizedCaseInsensitiveCompare&lt;T>(T) -> ComparisonResult

Compares the string and the given string using a case-insensitive, localized, comparison.

func localizedCaseInsensitiveContains&lt;T>(T) -> Bool

Returns a Boolean value indicating whether the given string is non-empty and contained within this string by case-insensitive, non-literal search, taking into account the current locale.

func localizedCompare&lt;T>(T) -> ComparisonResult

Compares the string and the given string using a localized comparison.

func localizedStandardCompare&lt;T>(T) -> ComparisonResult

Compares the string and the given string as sorted by the Finder.

func localizedStandardContains&lt;T>(T) -> Bool

Returns a Boolean value indicating whether the string contains the given string, taking the current locale into account.

func localizedStandardRange&lt;T>(of: T) -> Range&lt;Self.Index>?

Finds and returns the range of the first occurrence of a given string, taking the current locale into account. Returns `nil` if the string was not found.

func lowercased() -> String

**Required**

func lowercased(with: Locale?) -> String

Returns a version of the string with all letters converted to lowercase, taking into account the specified locale.

func maximumLengthOfBytes(using: String.Encoding) -> Int

Returns the maximum number of bytes needed to store the `String` in a given encoding.

func padding&lt;T>(toLength: Int, withPad: T, startingAt: Int) -> String

Returns a new string formed from the `String` by either removing characters from the end, or by appending as many occurrences as necessary of a given pad string.

func paragraphRange(for: some RangeExpression&lt;String.Index>) -> Range&lt;Self.Index>

Returns the range of characters representing the paragraph or paragraphs containing a given range.

func propertyList() -> Any

Parses the `String` as a text representation of a property list, returning an NSString, NSData, NSArray, or NSDictionary object, according to the topmost element.

func propertyListFromStringsFileFormat() -> [String : String]

Returns a dictionary object initialized with the keys and values found in the `String`.

func range&lt;T>(of: T, options: String.CompareOptions, range: Range&lt;Self.Index>?, locale: Locale?) -> Range&lt;Self.Index>?

Finds and returns the range of the first occurrence of a given string within a given range of the `String`, subject to given options, using the specified locale, if any.

func rangeOfCharacter(from: CharacterSet, options: String.CompareOptions, range: Range&lt;Self.Index>?) -> Range&lt;Self.Index>?

Finds and returns the range in the `String` of the first character from a given character set found in a given range with given options.

func rangeOfComposedCharacterSequence(at: Self.Index) -> Range&lt;Self.Index>

Returns the range in the `String` of the composed character sequence located at a given index.

func rangeOfComposedCharacterSequences&lt;R>(for: R) -> Range&lt;Self.Index>

Returns the range in the string of the composed character sequences for a given range.

func replacingCharacters&lt;T, R>(in: R, with: T) -> String

Returns a new string in which the characters in a specified range of the `String` are replaced by a given string.

func replacingOccurrences&lt;Target, Replacement>(of: Target, with: Replacement, options: String.CompareOptions, range: Range&lt;Self.Index>?) -> String

Returns a new string in which all occurrences of a target string in a specified range of the string are replaced by another given string.

func replacingPercentEscapes(using: String.Encoding) -> String?

Returns a new string made by replacing in the `String` all percent escapes with the matching characters as determined by a given encoding.

func split(separator: String, maxSplits: Int, omittingEmptySubsequences: Bool) -> [Substring]

func split(separator: Substring, maxSplits: Int, omittingEmptySubsequences: Bool) -> [Substring]

func substring(from: Self.Index) -> String

Returns a new string containing the characters of the `String` from the one at a given index to the end.

func substring(to: Self.Index) -> String

Returns a new string containing the characters of the `String` up to, but not including, the one at a given index.

func substring(with: Range&lt;Self.Index>) -> String

Returns a string object containing the characters of the `String` that lie within a given range.

func trimmingCharacters(in: CharacterSet) -> String

Returns a new string made by removing from both ends of the `String` characters contained in a given character set.

func uppercased() -> String

**Required**

func uppercased(with: Locale?) -> String

Returns a version of the string with all letters converted to uppercase, taking into account the specified locale.

func withCString&lt;Result>((UnsafePointer&lt;CChar>) throws -> Result) rethrows -> Result

Calls the given closure with a pointer to the contents of the string, represented as a null-terminated sequence of UTF-8 code units.

**Required**

func withCString&lt;Result, Encoding>(encodedAs: Encoding.Type, (UnsafePointer&lt;Encoding.CodeUnit>) throws -> Result) rethrows -> Result

Calls the given closure with a pointer to the contents of the string, represented as a null-terminated sequence of code units.

**Required**

func write(to: URL, atomically: Bool, encoding: String.Encoding) throws

Writes the contents of the `String` to the URL specified by url using the specified encoding.

func write&lt;T>(toFile: T, atomically: Bool, encoding: String.Encoding) throws

Writes the contents of the `String` to a file at a given path using a given encoding.

## Relationships

### Inherits From

- BidirectionalCollection
- Collection
- Comparable
- CustomStringConvertible
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- LosslessStringConvertible
- Sequence
- TextOutputStream
- TextOutputStreamable

### Conforming Types

- String
- Substring

## See Also

### Related String Types

struct Substring

A slice of a string.

struct Index

A position of a character or code unit in a string.

struct UnicodeScalarView

A view of a string’s contents as a collection of Unicode scalar values.

struct UTF16View

A view of a string’s contents as a collection of UTF-16 code units.

struct UTF8View

A view of a string’s contents as a collection of UTF-8 code units.

struct Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

struct Encoding

