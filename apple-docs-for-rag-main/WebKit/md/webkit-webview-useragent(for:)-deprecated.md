

- WebKit
- WebView
-  userAgent(for:) Deprecated

Instance Method

# userAgent(for:)

Returns the appropriate user-agent string for a given URL.

macOS 10.3–10.14Deprecated

``` source
@MainActor
func userAgent(for URL: URL!) -> String!
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`URL`  

The URL that you need the user-agent string for.

## Return Value

The user-agent string for a given URL. The user-agent string is used by websites to identify the client browser.

## See Also

### Getting and Setting User-agent Strings

var applicationNameForUserAgent: String!

The receiver’s application name that is used in the user-agent string.

Deprecated

var customUserAgent: String!

The receiver’s custom user-agent string.

Deprecated

