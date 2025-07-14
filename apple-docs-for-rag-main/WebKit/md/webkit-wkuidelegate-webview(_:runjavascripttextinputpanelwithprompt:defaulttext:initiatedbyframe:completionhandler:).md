

- WebKit
- WKUIDelegate
-  webView(\_:runJavaScriptTextInputPanelWithPrompt:defaultText:initiatedByFrame:completionHandler:) 

Instance Method

# webView(\_:runJavaScriptTextInputPanelWithPrompt:defaultText:initiatedByFrame:completionHandler:)

Displays a JavaScript text input panel.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    runJavaScriptTextInputPanelWithPrompt prompt: String,
    defaultText: String?,
    initiatedByFrame frame: WKFrameInfo,
    completionHandler: @escaping @MainActor (String?) -> Void
)
```

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    runJavaScriptTextInputPanelWithPrompt prompt: String,
    defaultText: String?,
    initiatedByFrame frame: WKFrameInfo
) async -> String?
```

## Parameters 

`webView`  

The web view invoking the delegate method.

`prompt`  

The message to be displayed.

`defaultText`  

The initial text to display in the text entry field.

`frame`  

Information about the frame whose JavaScript process initiated this call.

`completionHandler`  

The completion handler to call after the text input panel has been dismissed. Pass the entered text if the user chose OK, otherwise `nil`.

## Discussion

For user security, implementations of this method should call attention to the fact that a specific website controls the content in this panel. A simple formula for identifying the controlling website is `frame.request.URL.host`. The panel should have two buttons (typically OK and Cancel) and a field in which to enter text.

## See Also

### Displaying UI panels

func webView(WKWebView, runJavaScriptAlertPanelWithMessage: String, initiatedByFrame: WKFrameInfo, completionHandler: () -> Void)

Displays a JavaScript alert panel.

func webView(WKWebView, runJavaScriptConfirmPanelWithMessage: String, initiatedByFrame: WKFrameInfo, completionHandler: (Bool) -> Void)

Displays a JavaScript confirm panel.

func webView(WKWebView, showLockdownModeFirstUseMessage: String, completionHandler: (WKDialogResult) -> Void)

Displays a custom Lockdown Mode first use message.

enum WKDialogResult

An enumeration that lists the possible ways a delegate handled displaying a custom Lockdown Mode first use dialog.

