

- WebKit
- WebView
-  policyDelegate Deprecated

Instance Property

# policyDelegate

The receiver’s policy delegate.

macOS 10.3–10.14Deprecated

``` source
@MainActor
unowned(unsafe) var policyDelegate: (any WebPolicyDelegate)! { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

Conforms to the WebPolicyDelegate protocol.

## See Also

### Getting and Setting Delegates

var downloadDelegate: (any WebDownloadDelegate)!

The receiver’s download delegate.

Deprecated

var frameLoadDelegate: (any WebFrameLoadDelegate)!

The receiver’s frame load delegate.

Deprecated

var resourceLoadDelegate: (any WebResourceLoadDelegate)!

The receiver’s resource load delegate.

Deprecated

var uiDelegate: (any WebUIDelegate)!

The receiver’s user interface delegate.

Deprecated

