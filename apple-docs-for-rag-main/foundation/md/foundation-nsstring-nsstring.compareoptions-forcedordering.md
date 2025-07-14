

- Foundation
- NSString
- NSString.CompareOptions
-  forcedOrdering 

Type Property

# forcedOrdering

Comparisons are forced to return either `NSOrderedAscending` or `NSOrderedDescending` if the strings are equivalent but not strictly equal.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var forcedOrdering: NSString.CompareOptions { get }
```

## Discussion

This option ensures reliable, reproducible results when sorting. For example, “aaa” is greater than “AAA” if caseInsensitive is specified.

## See Also

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

