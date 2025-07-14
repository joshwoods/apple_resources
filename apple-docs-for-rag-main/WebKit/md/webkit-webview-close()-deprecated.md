

- WebKit
- WebView
-  close() Deprecated

Instance Method

# close()

Closes the web view when it’s no longer needed.

macOS 10.3–10.14Deprecated

``` source
@MainActor
func close()
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

Closes the web view by unloading its webpage and canceling any pending load requests. A closed web view no longer responds to new requests nor sends delegate messages. It is invoked automatically if the receiver’s enclosing window or host window is closed and sending shouldCloseWithWindow to the receiver returns true. Use this method to stop the receiver from loading and sending delegate messages.

## See Also

### Closing the View

var shouldCloseWithWindow: Bool

A Boolean that indicates whether the web view should close when its window or host window closes.

Deprecated

