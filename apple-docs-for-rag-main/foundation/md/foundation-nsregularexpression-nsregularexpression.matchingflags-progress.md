

- Foundation
- NSRegularExpression
- NSRegularExpression.MatchingFlags
-  progress 

Type Property

# progress

Set when the Block is called to report progress during a long-running match operation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var progress: NSRegularExpression.MatchingFlags { get }
```

## See Also

### Constants

static var completed: NSRegularExpression.MatchingFlags

Set when the Block is called after matching has completed.

static var hitEnd: NSRegularExpression.MatchingFlags

Set when the current match operation reached the end of the search range.

static var requiredEnd: NSRegularExpression.MatchingFlags

Set when the current match depended on the location of the end of the search range.

static var internalError: NSRegularExpression.MatchingFlags

Set when matching failed due to an internal error.

static var completed: NSRegularExpression.MatchingFlags

Set when the Block is called after matching has completed.

static var hitEnd: NSRegularExpression.MatchingFlags

Set when the current match operation reached the end of the search range.

static var requiredEnd: NSRegularExpression.MatchingFlags

Set when the current match depended on the location of the end of the search range.

static var internalError: NSRegularExpression.MatchingFlags

Set when matching failed due to an internal error.

