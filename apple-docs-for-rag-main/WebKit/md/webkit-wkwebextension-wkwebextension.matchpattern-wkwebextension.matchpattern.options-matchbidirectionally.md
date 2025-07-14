

- WebKit
- WKWebExtension
- WKWebExtension.MatchPattern
- WKWebExtension.MatchPattern.Options
-  matchBidirectionally 

Type Property

# matchBidirectionally

Indicates that two patterns should be checked in either direction while matching.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
static var matchBidirectionally: WKWebExtension.MatchPattern.Options { get }
```

## Discussion

For example, A matches B, or B matches A. Invalid for matching URLs.

