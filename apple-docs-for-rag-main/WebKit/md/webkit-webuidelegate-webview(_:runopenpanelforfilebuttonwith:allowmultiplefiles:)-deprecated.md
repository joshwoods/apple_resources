

- WebKit
- WebUIDelegate
-  webView(\_:runOpenPanelForFileButtonWith:allowMultipleFiles:) Deprecated

Instance Method

# webView(\_:runOpenPanelForFileButtonWith:allowMultipleFiles:)

Displays an open panel for a file input control.

macOS 10.6–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    runOpenPanelForFileButtonWith resultListener: (any WebOpenPanelResultListener)!,
    allowMultipleFiles: Bool
)
```

## Parameters 

`sender`  

The web view that sent the message.

`resultListener`  

See the WebOpenPanelResultListener protocol for how to set these values.

`allowMultipleFiles`  

If true, the open panel should allow multiple files to be selected; otherwise, it should not.

## See Also

### Opening Panels

func webView(WebView!, runJavaScriptAlertPanelWithMessage: String!, initiatedBy: WebFrame!)

Displays a JavaScript alert panel containing the specified message.

Deprecated

func webView(WebView!, runJavaScriptConfirmPanelWithMessage: String!, initiatedBy: WebFrame!) -> Bool

Displays a JavaScript confirmation panel with the specified message.

Deprecated

func webView(WebView!, runJavaScriptTextInputPanelWithPrompt: String!, defaultText: String!, initiatedBy: WebFrame!) -> String!

Displays a JavaScript text input panel and returns the entered text.

Deprecated

func webView(WebView!, runOpenPanelForFileButtonWith: (any WebOpenPanelResultListener)!)

Displays an open panel for a file input control.

Deprecated

func webView(WebView!, runBeforeUnloadConfirmPanelWithMessage: String!, initiatedBy: WebFrame!) -> Bool

Displays a confirmation panel containing the specified message before a window closes.

Deprecated

