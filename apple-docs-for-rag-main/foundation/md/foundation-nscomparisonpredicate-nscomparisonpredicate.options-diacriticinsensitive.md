

- Foundation
- NSComparisonPredicate
- NSComparisonPredicate.Options
-  diacriticInsensitive 

Type Property

# diacriticInsensitive

A diacritic-insensitive predicate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var diacriticInsensitive: NSComparisonPredicate.Options { get }
```

## Discussion

You represent this option in a predicate format string using a `[d]` following a string operation (for example, `"naïve" like[d] "naive"`).

## See Also

### Constants

static var caseInsensitive: NSComparisonPredicate.Options

A case-insensitive predicate.

static var normalized: NSComparisonPredicate.Options

A predicate that indicates you’ve preprocessed the strings to compare.

static var caseInsensitive: NSComparisonPredicate.Options

A case-insensitive predicate.

static var normalized: NSComparisonPredicate.Options

A predicate that indicates you’ve preprocessed the strings to compare.

