

- WebKit
- WebUIDelegate
-  webView(\_:runBeforeUnloadConfirmPanelWithMessage:initiatedBy:) Deprecated

Instance Method

# webView(\_:runBeforeUnloadConfirmPanelWithMessage:initiatedBy:)

Displays a confirmation panel containing the specified message before a window closes.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    runBeforeUnloadConfirmPanelWithMessage message: String!,
    initiatedBy frame: WebFrame!
) -> Bool
```

## Parameters 

`sender`  

The web view that sent the message.

`message`  

The message to display in the panel.

`frame`  

The web frame whose JavaScript initiated this call.

## Return Value

true if the user clicked the OK button; otherwise, false.

## Discussion

Use this method to include a message in the confirmation panel in addition to the message supplied by the webpage. The confirmation panel should contain OK and Cancel buttons.

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

func webView(WebView!, runOpenPanelForFileButtonWith: (any WebOpenPanelResultListener)!, allowMultipleFiles: Bool)

Displays an open panel for a file input control.

Deprecated

