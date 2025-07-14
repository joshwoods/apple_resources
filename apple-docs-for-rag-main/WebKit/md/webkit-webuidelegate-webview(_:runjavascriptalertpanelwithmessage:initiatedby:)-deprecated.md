

- WebKit
- WebUIDelegate
-  webView(\_:runJavaScriptAlertPanelWithMessage:initiatedBy:) Deprecated

Instance Method

# webView(\_:runJavaScriptAlertPanelWithMessage:initiatedBy:)

Displays a JavaScript alert panel containing the specified message.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    runJavaScriptAlertPanelWithMessage message: String!,
    initiatedBy frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view that sent the message.

`message`  

The message to display in the alert panel.

`frame`  

The web frame whose JavaScript initiated this call.

## Discussion

This method displays an alert panel when JavaScript code calls `alert`. Delegates should visually indicate that this panel comes from JavaScript. The panel should contain a single OK button. No action is taken if you do not implement this method.

## See Also

### Opening Panels

func webView(WebView!, runJavaScriptConfirmPanelWithMessage: String!, initiatedBy: WebFrame!) -> Bool

Displays a JavaScript confirmation panel with the specified message.

Deprecated

func webView(WebView!, runJavaScriptTextInputPanelWithPrompt: String!, defaultText: String!, initiatedBy: WebFrame!) -> String!

Displays a JavaScript text input panel and returns the entered text.

Deprecated

func webView(WebView!, runOpenPanelForFileButtonWith: (any WebOpenPanelResultListener)!)

Displays an open panel for a file input control.

Deprecated

func webView(WebView!, runOpenPanelForFileButtonWith: (any WebOpenPanelResultListener)!, allowMultipleFiles: Bool)

Displays an open panel for a file input control.

Deprecated

func webView(WebView!, runBeforeUnloadConfirmPanelWithMessage: String!, initiatedBy: WebFrame!) -> Bool

Displays a confirmation panel containing the specified message before a window closes.

Deprecated

