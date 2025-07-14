

- Foundation
- NSRegularExpression
-  NSRegularExpression.MatchingFlags 

Structure

# NSRegularExpression.MatchingFlags

Set by the Block as the matching progresses, completes, or fails. Used by the method enumerateMatches(in:options:range:using:).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct MatchingFlags
```

## Topics

### Constants

static var progress: NSRegularExpression.MatchingFlags

Set when the Block is called to report progress during a long-running match operation.

static var completed: NSRegularExpression.MatchingFlags

Set when the Block is called after matching has completed.

static var hitEnd: NSRegularExpression.MatchingFlags

Set when the current match operation reached the end of the search range.

static var requiredEnd: NSRegularExpression.MatchingFlags

Set when the current match depended on the location of the end of the search range.

static var internalError: NSRegularExpression.MatchingFlags

Set when matching failed due to an internal error.

static var progress: NSRegularExpression.MatchingFlags

Set when the Block is called to report progress during a long-running match operation.

static var completed: NSRegularExpression.MatchingFlags

Set when the Block is called after matching has completed.

static var hitEnd: NSRegularExpression.MatchingFlags

Set when the current match operation reached the end of the search range.

static var requiredEnd: NSRegularExpression.MatchingFlags

Set when the current match depended on the location of the end of the search range.

static var internalError: NSRegularExpression.MatchingFlags

Set when matching failed due to an internal error.

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

### Constants

struct Options

These constants define the regular expression options. These constants are used by the property options, regularExpressionWithPattern:options:error:, and init(pattern:options:).

struct MatchingOptions

The matching options constants specify the reporting, completion and matching rules to the expression matching methods. These constants are used by all methods that search for, or replace values, using a regular expression.

