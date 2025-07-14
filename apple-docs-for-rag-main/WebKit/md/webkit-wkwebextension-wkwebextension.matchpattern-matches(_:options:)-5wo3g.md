

- WebKit
- WKWebExtension
- WKWebExtension.MatchPattern
-  matches(\_:options:) 

Instance Method

# matches(\_:options:)

Matches the receiver pattern against the specified URL with options.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func matches(
    _ url: URL?,
    options: WKWebExtension.MatchPattern.Options = []
) -> Bool
```

## Parameters 

`url`  

The URL to match against the receiver pattern.

`options`  

The options to use while matching.

## Return Value

A Boolean value indicating if the pattern matches the specified URL.

## See Also

### Related Documentation

func matches(URL?) -> Bool

Matches the receiver pattern against the specified URL.

