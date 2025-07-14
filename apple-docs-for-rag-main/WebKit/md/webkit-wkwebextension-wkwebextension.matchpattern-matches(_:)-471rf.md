

- WebKit
- WKWebExtension
- WKWebExtension.MatchPattern
-  matches(\_:) 

Instance Method

# matches(\_:)

Matches the receiver pattern against the specified URL.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func matches(_ url: URL?) -> Bool
```

## Parameters 

`url`  

The URL to match against the receiver pattern.

## Return Value

A Boolean value indicating if the pattern matches the specified URL.

## See Also

### Related Documentation

func matches(URL?, options: WKWebExtension.MatchPattern.Options) -> Bool

Matches the receiver pattern against the specified URL with options.

