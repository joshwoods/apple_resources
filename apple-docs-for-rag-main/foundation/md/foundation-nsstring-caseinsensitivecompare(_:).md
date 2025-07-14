

- Foundation
- NSString
-  caseInsensitiveCompare(\_:) 

Instance Method

# caseInsensitiveCompare(\_:)

Returns the result of invoking compare(_:options:) with `NSCaseInsensitiveSearch` as the only option.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func caseInsensitiveCompare(_ string: String) -> ComparisonResult
```

## Parameters 

`string`  

The string with which to compare the receiver.

## Return Value

Returns an ComparisonResult value that indicates the lexical ordering. ComparisonResult.orderedAscending the receiver precedes `aString` in lexical ordering, ComparisonResult.orderedSame the receiver and `aString` are equivalent in lexical value, and ComparisonResult.orderedDescending if the receiver follows `aString`.

## Discussion

This method is the equivalent of invoking compare(_:options:) with caseInsensitive as the only option.

Important

When working with text that’s presented to the user, use the localizedCaseInsensitiveCompare(_:) method instead.

## See Also

### Identifying and Comparing Strings

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

struct CompareOptions

These values represent the options available to many of the string classes’ search and comparison methods.

struct EncodingConversionOptions

Options for converting string encodings.

