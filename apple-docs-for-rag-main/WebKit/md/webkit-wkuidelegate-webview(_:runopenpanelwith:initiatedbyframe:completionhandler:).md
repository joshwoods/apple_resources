

- WebKit
- WKUIDelegate
-  webView(\_:runOpenPanelWith:initiatedByFrame:completionHandler:) 

Instance Method

# webView(\_:runOpenPanelWith:initiatedByFrame:completionHandler:)

Displays a file upload panel.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 10.12+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    runOpenPanelWith parameters: WKOpenPanelParameters,
    initiatedByFrame frame: WKFrameInfo,
    completionHandler: @escaping @MainActor ([URL]?) -> Void
)
```

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    runOpenPanelWith parameters: WKOpenPanelParameters,
    initiatedByFrame frame: WKFrameInfo
) async -> [URL]?
```

## Parameters 

`webView`  

The web view invoking the delegate method.

`parameters`  

The parameters describing the file upload control.

`frame`  

The frame whose file upload control initiated the call.

`completionHandler`  

The completion handler called after the open panel has been dismissed. Pass the selected URLs if the user chose “OK”, otherwise `nil`.

## Discussion

If this method is not implemented, the web view behaves as if the user selected the Cancel button.

## See Also

### Displaying an upload panel

class WKOpenPanelParameters

The configuration details of a file upload control in your web content.

