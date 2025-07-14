

- WebKit
- WebView
-  customUserAgent Deprecated

Instance Property

# customUserAgent

The receiver’s custom user-agent string.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var customUserAgent: String! { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

The custom user-agent string is used for all URLs. If `nil`, then the receiver constructs a user-agent string that produces the best rendering results for each URL.

## See Also

### Getting and Setting User-agent Strings

func userAgent(for: URL!) -> String!

Returns the appropriate user-agent string for a given URL.

Deprecated

var applicationNameForUserAgent: String!

The receiver’s application name that is used in the user-agent string.

Deprecated

