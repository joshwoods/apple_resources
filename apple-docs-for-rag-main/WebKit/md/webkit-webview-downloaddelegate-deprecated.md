

- WebKit
- WebView
-  downloadDelegate Deprecated

Instance Property

# downloadDelegate

The receiver’s download delegate.

macOS 10.3–10.14Deprecated

``` source
@MainActor
unowned(unsafe) var downloadDelegate: (any WebDownloadDelegate)! { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

Implements the WebDownload protocol.

WebKit may create `WebDownload` objects automatically to handle downloads that start with a webpage or link.

## See Also

### Getting and Setting Delegates

var frameLoadDelegate: (any WebFrameLoadDelegate)!

The receiver’s frame load delegate.

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

