

- WebKit
- WebUIDelegate
-  webView(\_:runJavaScriptTextInputPanelWithPrompt:defaultText:initiatedBy:) Deprecated

Instance Method

# webView(\_:runJavaScriptTextInputPanelWithPrompt:defaultText:initiatedBy:)

Displays a JavaScript text input panel and returns the entered text.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    runJavaScriptTextInputPanelWithPrompt prompt: String!,
    defaultText: String!,
    initiatedBy frame: WebFrame!
) -> String!
```

## Parameters 

`sender`  

The web view that sent the message.

`prompt`  

The message to display in the text input panel.

`defaultText`  

Default placeholder text to display in the text field.

`frame`  

The web frame whose JavaScript initiated this call.

## Return Value

The text entered by the user if the user clicks OK; otherwise, `nil`.

## Discussion

This method is used to provide an alternate text input panel when JavaScript code calls `prompt`. Delegates should visually indicate that this panel comes from JavaScript. The panel should contain an OK and a Cancel button, and an editable text field. If you do not implement this method, a JavaScript text input panel is displayed.

## See Also

### Opening Panels

func webView(WebView!, runJavaScriptAlertPanelWithMessage: String!, initiatedBy: WebFrame!)

Displays a JavaScript alert panel containing the specified message.

Deprecated

func webView(WebView!, runJavaScriptConfirmPanelWithMessage: String!, initiatedBy: WebFrame!) -> Bool

Displays a JavaScript confirmation panel with the specified message.

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

