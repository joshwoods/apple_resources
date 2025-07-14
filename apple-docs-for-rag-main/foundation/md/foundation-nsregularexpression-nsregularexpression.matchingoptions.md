

- Foundation
- NSRegularExpression
-  NSRegularExpression.MatchingOptions 

Structure

# NSRegularExpression.MatchingOptions

The matching options constants specify the reporting, completion and matching rules to the expression matching methods. These constants are used by all methods that search for, or replace values, using a regular expression.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct MatchingOptions
```

## Topics

### Constants

static var reportProgress: NSRegularExpression.MatchingOptions

Call the Block periodically during long-running match operations. This option has no effect for methods other than enumerateMatches(in:options:range:using:). See enumerateMatches(in:options:range:using:) for a description of the constant in context.

static var reportCompletion: NSRegularExpression.MatchingOptions

Call the Block once after the completion of any matching. This option has no effect for methods other than enumerateMatches(in:options:range:using:). See enumerateMatches(in:options:range:using:) for a description of the constant in context.

static var anchored: NSRegularExpression.MatchingOptions

Specifies that matches are limited to those at the start of the search range. See enumerateMatches(in:options:range:using:) for a description of the constant in context.

static var withTransparentBounds: NSRegularExpression.MatchingOptions

Specifies that matching may examine parts of the string beyond the bounds of the search range, for purposes such as word boundary detection, lookahead, etc. This constant has no effect if the search range contains the entire string. See enumerateMatches(in:options:range:using:) for a description of the constant in context.

static var withoutAnchoringBounds: NSRegularExpression.MatchingOptions

Specifies that `^` and `$` will not automatically match the beginning and end of the search range, but will still match the beginning and end of the entire string. This constant has no effect if the search range contains the entire string. See enumerateMatches(in:options:range:using:) for a description of the constant in context.

static var reportProgress: NSRegularExpression.MatchingOptions

Call the Block periodically during long-running match operations. This option has no effect for methods other than enumerateMatches(in:options:range:using:). See enumerateMatches(in:options:range:using:) for a description of the constant in context.

static var reportCompletion: NSRegularExpression.MatchingOptions

Call the Block once after the completion of any matching. This option has no effect for methods other than enumerateMatches(in:options:range:using:). See enumerateMatches(in:options:range:using:) for a description of the constant in context.

static var anchored: NSRegularExpression.MatchingOptions

Specifies that matches are limited to those at the start of the search range. See enumerateMatches(in:options:range:using:) for a description of the constant in context.

static var withTransparentBounds: NSRegularExpression.MatchingOptions

Specifies that matching may examine parts of the string beyond the bounds of the search range, for purposes such as word boundary detection, lookahead, etc. This constant has no effect if the search range contains the entire string. See enumerateMatches(in:options:range:using:) for a description of the constant in context.

static var withoutAnchoringBounds: NSRegularExpression.MatchingOptions

Specifies that `^` and `$` will not automatically match the beginning and end of the search range, but will still match the beginning and end of the entire string. This constant has no effect if the search range contains the entire string. See enumerateMatches(in:options:range:using:) for a description of the constant in context.

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

struct MatchingFlags

Set by the Block as the matching progresses, completes, or fails. Used by the method enumerateMatches(in:options:range:using:).

