

- Foundation
- NSRegularExpression
-  NSRegularExpression.Options 

Structure

# NSRegularExpression.Options

These constants define the regular expression options. These constants are used by the property options, regularExpressionWithPattern:options:error:, and init(pattern:options:).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Options
```

## Topics

### Constants

static var caseInsensitive: NSRegularExpression.Options

Match letters in the pattern independent of case.

static var allowCommentsAndWhitespace: NSRegularExpression.Options

Ignore whitespace and \#-prefixed comments in the pattern.

static var ignoreMetacharacters: NSRegularExpression.Options

Treat the entire pattern as a literal string.

static var dotMatchesLineSeparators: NSRegularExpression.Options

Allow `.` to match any character, including line separators.

static var anchorsMatchLines: NSRegularExpression.Options

Allow `^` and `$` to match the start and end of lines.

static var useUnixLineSeparators: NSRegularExpression.Options

Treat only `\n` as a line separator (otherwise, all standard line separators are used).

static var useUnicodeWordBoundaries: NSRegularExpression.Options

Use Unicode `TR#29` to specify word boundaries (otherwise, traditional regular expression word boundaries are used).

static var caseInsensitive: NSRegularExpression.Options

Match letters in the pattern independent of case.

static var allowCommentsAndWhitespace: NSRegularExpression.Options

Ignore whitespace and \#-prefixed comments in the pattern.

static var ignoreMetacharacters: NSRegularExpression.Options

Treat the entire pattern as a literal string.

static var dotMatchesLineSeparators: NSRegularExpression.Options

Allow `.` to match any character, including line separators.

static var anchorsMatchLines: NSRegularExpression.Options

Allow `^` and `$` to match the start and end of lines.

static var useUnixLineSeparators: NSRegularExpression.Options

Treat only `\n` as a line separator (otherwise, all standard line separators are used).

static var useUnicodeWordBoundaries: NSRegularExpression.Options

Use Unicode `TR#29` to specify word boundaries (otherwise, traditional regular expression word boundaries are used).

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

struct MatchingFlags

Set by the Block as the matching progresses, completes, or fails. Used by the method enumerateMatches(in:options:range:using:).

struct MatchingOptions

The matching options constants specify the reporting, completion and matching rules to the expression matching methods. These constants are used by all methods that search for, or replace values, using a regular expression.

