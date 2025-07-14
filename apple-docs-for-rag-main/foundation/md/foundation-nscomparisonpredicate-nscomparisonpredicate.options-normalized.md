

- Foundation
- NSComparisonPredicate
- NSComparisonPredicate.Options
-  normalized 

Type Property

# normalized

A predicate that indicates you’ve preprocessed the strings to compare.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var normalized: NSComparisonPredicate.Options { get }
```

## Discussion

This option supersedes `NSCaseInsensitivePredicateOption` and `NSDiacriticInsensitivePredicateOption`, and is a performance optimization option.

You represent this option in a predicate format string using a `[n]` following a string operation (for example, `"WXYZlan" matches[n] ".lan"`).

## See Also

### Constants

static var caseInsensitive: NSComparisonPredicate.Options

A case-insensitive predicate.

static var diacriticInsensitive: NSComparisonPredicate.Options

A diacritic-insensitive predicate.

static var caseInsensitive: NSComparisonPredicate.Options

A case-insensitive predicate.

static var diacriticInsensitive: NSComparisonPredicate.Options

A diacritic-insensitive predicate.

