

- Foundation
- NSString
-  NSString.CompareOptions 

Structure

# NSString.CompareOptions

These values represent the options available to many of the string classes’ search and comparison methods.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct CompareOptions
```

## Overview

See Searching, Comparing, and Sorting Strings for details on the effects of these options.

## Topics

### Constants

static var caseInsensitive: NSString.CompareOptions

A case-insensitive search.

static var literal: NSString.CompareOptions

Exact character-by-character equivalence.

static var backwards: NSString.CompareOptions

Search from end of source string.

static var anchored: NSString.CompareOptions

Search is limited to start (or end, if `NSBackwardsSearch`) of source string.

static var numeric: NSString.CompareOptions

Numbers within strings are compared using numeric value, that is, `Name2.txt` \

static var diacriticInsensitive: NSString.CompareOptions

Search ignores diacritic marks.

static var widthInsensitive: NSString.CompareOptions

Search ignores width differences in characters that have full-width and half-width forms, as occurs in East Asian character sets.

static var forcedOrdering: NSString.CompareOptions

Comparisons are forced to return either `NSOrderedAscending` or `NSOrderedDescending` if the strings are equivalent but not strictly equal.

static var regularExpression: NSString.CompareOptions

The search string is treated as an ICU-compatible regular expression. If set, no other options can apply except caseInsensitive and anchored. You can use this option only with the `rangeOfString:`… methods and replacingOccurrences(of:with:options:range:).

static var caseInsensitive: NSString.CompareOptions

A case-insensitive search.

static var literal: NSString.CompareOptions

Exact character-by-character equivalence.

static var backwards: NSString.CompareOptions

Search from end of source string.

static var anchored: NSString.CompareOptions

Search is limited to start (or end, if `NSBackwardsSearch`) of source string.

static var numeric: NSString.CompareOptions

Numbers within strings are compared using numeric value, that is, `Name2.txt` \

static var diacriticInsensitive: NSString.CompareOptions

Search ignores diacritic marks.

static var widthInsensitive: NSString.CompareOptions

Search ignores width differences in characters that have full-width and half-width forms, as occurs in East Asian character sets.

static var forcedOrdering: NSString.CompareOptions

Comparisons are forced to return either `NSOrderedAscending` or `NSOrderedDescending` if the strings are equivalent but not strictly equal.

static var regularExpression: NSString.CompareOptions

The search string is treated as an ICU-compatible regular expression. If set, no other options can apply except caseInsensitive and anchored. You can use this option only with the `rangeOfString:`… methods and replacingOccurrences(of:with:options:range:).

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Identifying and Comparing Strings

func caseInsensitiveCompare(String) -> ComparisonResult

Returns the result of invoking compare(_:options:) with `NSCaseInsensitiveSearch` as the only option.

func localizedCaseInsensitiveCompare(String) -> ComparisonResult

Compares the string with a given string using a case-insensitive, localized, comparison.

func compare(String) -> ComparisonResult

Returns the result of invoking compare(_:options:range:) with no options and the receiver’s full extent as the range.

func localizedCompare(String) -> ComparisonResult

Compares the string and a given string using a localized comparison.

func compare(String, options: NSString.CompareOptions) -> ComparisonResult

Compares the string with the specified string using the given options.

func compare(String, options: NSString.CompareOptions, range: NSRange) -> ComparisonResult

Returns the result of invoking compare(_:options:range:locale:) with a `nil` locale.

func compare(String, options: NSString.CompareOptions, range: NSRange, locale: Any?) -> ComparisonResult

Compares the string using the specified options and returns the lexical ordering for the range.

func localizedStandardCompare(String) -> ComparisonResult

Compares strings as sorted by the Finder.

func hasPrefix(String) -> Bool

Returns a Boolean value that indicates whether a given string matches the beginning characters of the receiver.

func hasSuffix(String) -> Bool

Returns a Boolean value that indicates whether a given string matches the ending characters of the receiver.

func isEqual(to: String) -> Bool

Returns a Boolean value that indicates whether a given string is equal to the receiver using a literal Unicode-based comparison.

var hash: Int

An unsigned integer that can be used as a hash table address.

struct EncodingConversionOptions

Options for converting string encodings.

