

- WebKit
- WKWebExtension
- WKWebExtension.MatchPattern
-  matches(\_:) 

Instance Method

# matches(\_:)

Matches the receiver pattern against the specified pattern.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func matches(_ pattern: WKWebExtension.MatchPattern?) -> Bool
```

## Parameters 

`pattern`  

The pattern to match against the receiver pattern.

## Return Value

A Boolean value indicating if the receiver pattern matches the specified pattern.

## See Also

### Related Documentation

func matches(WKWebExtension.MatchPattern?, options: WKWebExtension.MatchPattern.Options) -> Bool

Matches the receiver pattern against the specified pattern with options.

