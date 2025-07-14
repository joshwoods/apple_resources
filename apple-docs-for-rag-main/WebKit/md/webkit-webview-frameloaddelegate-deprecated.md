

- WebKit
- WebView
-  frameLoadDelegate Deprecated

Instance Property

# frameLoadDelegate

The receiver’s frame load delegate.

macOS 10.3–10.14Deprecated

``` source
@MainActor
unowned(unsafe) var frameLoadDelegate: (any WebFrameLoadDelegate)! { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

Conforms to the WebFrameLoadDelegate protocol.

## See Also

### Getting and Setting Delegates

var downloadDelegate: (any WebDownloadDelegate)!

The receiver’s download delegate.

Deprecated

var policyDelegate: (any WebPolicyDelegate)!

The receiver’s policy delegate.

Deprecated

var resourceLoadDelegate: (any WebResourceLoadDelegate)!

The receiver’s resource load delegate.

Deprecated

var uiDelegate: (any WebUIDelegate)!

The receiver’s user interface delegate.

Deprecated

