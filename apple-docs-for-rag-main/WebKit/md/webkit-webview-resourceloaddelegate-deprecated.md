

- WebKit
- WebView
-  resourceLoadDelegate Deprecated

Instance Property

# resourceLoadDelegate

The receiver’s resource load delegate.

macOS 10.3–10.14Deprecated

``` source
@MainActor
unowned(unsafe) var resourceLoadDelegate: (any WebResourceLoadDelegate)! { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

Conforms to the WebResourceLoadDelegate protocol.

## See Also

### Getting and Setting Delegates

var downloadDelegate: (any WebDownloadDelegate)!

The receiver’s download delegate.

Deprecated

var frameLoadDelegate: (any WebFrameLoadDelegate)!

The receiver’s frame load delegate.

Deprecated

var policyDelegate: (any WebPolicyDelegate)!

The receiver’s policy delegate.

Deprecated

var uiDelegate: (any WebUIDelegate)!

The receiver’s user interface delegate.

Deprecated

