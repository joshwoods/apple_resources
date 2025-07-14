

- WebKit
- WKUIDelegate
-  webView(\_:runJavaScriptConfirmPanelWithMessage:initiatedByFrame:completionHandler:) 

Instance Method

# webView(\_:runJavaScriptConfirmPanelWithMessage:initiatedByFrame:completionHandler:)

Displays a JavaScript confirm panel.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    runJavaScriptConfirmPanelWithMessage message: String,
    initiatedByFrame frame: WKFrameInfo,
    completionHandler: @escaping @MainActor (Bool) -> Void
)
```

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    runJavaScriptConfirmPanelWithMessage message: String,
    initiatedByFrame frame: WKFrameInfo
) async -> Bool
```

## Parameters 

`webView`  

The web view invoking the delegate method.

`message`  

The message to be displayed.

`frame`  

Information about the frame whose JavaScript process initiated this call.

`completionHandler`  

The completion handler to call after the confirm panel has been dismissed. Pass true if the user chose OK, and pass false if the user chose Cancel.

## Discussion

For user security, implementations of this method should call attention to the fact that a specific website controls the content in this panel. A simple formula for identifying the controlling website is `frame.request.URL.host`. The panel should have two buttons, typically OK and Cancel.

## See Also

### Displaying UI panels

func webView(WKWebView, runJavaScriptAlertPanelWithMessage: String, initiatedByFrame: WKFrameInfo, completionHandler: () -> Void)

Displays a JavaScript alert panel.

func webView(WKWebView, runJavaScriptTextInputPanelWithPrompt: String, defaultText: String?, initiatedByFrame: WKFrameInfo, completionHandler: (String?) -> Void)

Displays a JavaScript text input panel.

func webView(WKWebView, showLockdownModeFirstUseMessage: String, completionHandler: (WKDialogResult) -> Void)

Displays a custom Lockdown Mode first use message.

enum WKDialogResult

An enumeration that lists the possible ways a delegate handled displaying a custom Lockdown Mode first use dialog.

