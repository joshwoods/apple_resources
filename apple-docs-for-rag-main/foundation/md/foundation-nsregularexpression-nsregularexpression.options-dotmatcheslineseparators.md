

- Foundation
- NSRegularExpression
- NSRegularExpression.Options
-  dotMatchesLineSeparators 

Type Property

# dotMatchesLineSeparators

Allow `.` to match any character, including line separators.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var dotMatchesLineSeparators: NSRegularExpression.Options { get }
```

## See Also

### Constants

static var caseInsensitive: NSRegularExpression.Options

Match letters in the pattern independent of case.

static var allowCommentsAndWhitespace: NSRegularExpression.Options

Ignore whitespace and \#-prefixed comments in the pattern.

static var ignoreMetacharacters: NSRegularExpression.Options

Treat the entire pattern as a literal string.

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

static var anchorsMatchLines: NSRegularExpression.Options

Allow `^` and `$` to match the start and end of lines.

static var useUnixLineSeparators: NSRegularExpression.Options

Treat only `\n` as a line separator (otherwise, all standard line separators are used).

static var useUnicodeWordBoundaries: NSRegularExpression.Options

Use Unicode `TR#29` to specify word boundaries (otherwise, traditional regular expression word boundaries are used).

