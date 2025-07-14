

- WebKit
- WebView
-  uiDelegate Deprecated

Instance Property

# uiDelegate

The receiver’s user interface delegate.

macOS 10.3–10.14Deprecated

``` source
@MainActor
unowned(unsafe) var uiDelegate: (any WebUIDelegate)! { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

A user interface delegate that conforms to the WebUIDelegate protocol.

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

var resourceLoadDelegate: (any WebResourceLoadDelegate)!

The receiver’s resource load delegate.

Deprecated

