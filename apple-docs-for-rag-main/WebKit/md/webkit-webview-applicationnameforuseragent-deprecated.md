

- WebKit
- WebView
-  applicationNameForUserAgent Deprecated

Instance Property

# applicationNameForUserAgent

The receiver’s application name that is used in the user-agent string.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var applicationNameForUserAgent: String! { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

The user-agent is used by websites to identify the client browser.

## See Also

### Getting and Setting User-agent Strings

func userAgent(for: URL!) -> String!

Returns the appropriate user-agent string for a given URL.

Deprecated

var customUserAgent: String!

The receiver’s custom user-agent string.

Deprecated

