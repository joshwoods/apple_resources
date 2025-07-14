

- UIKit
- UIPasteboard
- UIPasteboard.DetectionPattern
-  probableWebSearch 

Type Property

# probableWebSearch

A pattern that indicates the pasteboard contains a string suitable for use as a web search term.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
static let probableWebSearch: UIPasteboard.DetectionPattern
```

## Discussion

When you include this pattern in calls to detectValues(for:inItemSet:completionHandler:) or detectValues(for:completionHandler:) — detectValuesForPatterns:inItemSet:completionHandler: or detectValuesForPatterns:completionHandler: in Objective-C — and the pasteboard detects a string suitable for use as a web search term, it reports the value as an NSString.

## See Also

### Detecting common patterns

static let number: UIPasteboard.DetectionPattern

A pattern that indicates the pasteboard contains a string that consists of a numeric value.

static let probableWebURL: UIPasteboard.DetectionPattern

A pattern that indicates the pasteboard contains a string that consists of a URL.

