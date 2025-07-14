

- WebKit
- WKUIDelegate
-  webView(\_:showLockdownModeFirstUseMessage:completionHandler:) 

Instance Method

# webView(\_:showLockdownModeFirstUseMessage:completionHandler:)

Displays a custom Lockdown Mode first use message.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    showLockdownModeFirstUseMessage message: String,
    completionHandler: @escaping @MainActor (WKDialogResult) -> Void
)
```

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    showLockdownModeFirstUseMessage message: String
) async -> WKDialogResult
```

## Parameters 

`webView`  

The web view that is requesting to display the Lockdown Mode first use dialog.

`message`  

The message for the web view to display if the delegate does not display the first use dialog.

`completionHandler`  

A block you must invoke to resume after the web view displays the first use dialog. The block does not return a value, and accepts the following parameter:

dialogResult  
A display result case that indicates how the method handled the display request.

## Discussion

Implement this method to display a custom Lockdown Mode message, or to suppress the message. Return, or call the completion handler, with a WKDialogResult case that indicates how your method handled the display request. For more information about Lockdown Mode, see About Lockdown Mode.

If you don’t implement this method, the web view displays the default message.

## See Also

### Displaying UI panels

func webView(WKWebView, runJavaScriptAlertPanelWithMessage: String, initiatedByFrame: WKFrameInfo, completionHandler: () -> Void)

Displays a JavaScript alert panel.

func webView(WKWebView, runJavaScriptConfirmPanelWithMessage: String, initiatedByFrame: WKFrameInfo, completionHandler: (Bool) -> Void)

Displays a JavaScript confirm panel.

func webView(WKWebView, runJavaScriptTextInputPanelWithPrompt: String, defaultText: String?, initiatedByFrame: WKFrameInfo, completionHandler: (String?) -> Void)

Displays a JavaScript text input panel.

enum WKDialogResult

An enumeration that lists the possible ways a delegate handled displaying a custom Lockdown Mode first use dialog.

