

- WebKit
- WKUIDelegate
-  webView(\_:runJavaScriptAlertPanelWithMessage:initiatedByFrame:completionHandler:) 

Instance Method

# webView(\_:runJavaScriptAlertPanelWithMessage:initiatedByFrame:completionHandler:)

Displays a JavaScript alert panel.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    runJavaScriptAlertPanelWithMessage message: String,
    initiatedByFrame frame: WKFrameInfo,
    completionHandler: @escaping @MainActor () -> Void
)
```

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    runJavaScriptAlertPanelWithMessage message: String,
    initiatedByFrame frame: WKFrameInfo
) async
```

## Parameters 

`webView`  

The web view invoking the delegate method.

`message`  

The message to be displayed.

`frame`  

Information about the frame whose JavaScript process initiated this call.

`completionHandler`  

The completion handler to call after the alert panel has been dismissed.

## Discussion

For user security, implementations of this method should call attention to the fact that a specific website controls the content in this panel. A simple formula for identifying the controlling website is `frame.request.URL.host`. The panel should have a single OK button.

## See Also

### Displaying UI panels

func webView(WKWebView, runJavaScriptConfirmPanelWithMessage: String, initiatedByFrame: WKFrameInfo, completionHandler: (Bool) -> Void)

Displays a JavaScript confirm panel.

func webView(WKWebView, runJavaScriptTextInputPanelWithPrompt: String, defaultText: String?, initiatedByFrame: WKFrameInfo, completionHandler: (String?) -> Void)

Displays a JavaScript text input panel.

func webView(WKWebView, showLockdownModeFirstUseMessage: String, completionHandler: (WKDialogResult) -> Void)

Displays a custom Lockdown Mode first use message.

enum WKDialogResult

An enumeration that lists the possible ways a delegate handled displaying a custom Lockdown Mode first use dialog.

