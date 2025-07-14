

- WebKit
-  WKDialogResult 

Enumeration

# WKDialogResult

An enumeration that lists the possible ways a delegate handled displaying a custom Lockdown Mode first use dialog.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
enum WKDialogResult
```

## Topics

### First use dialog results

case askAgain

A result that indicates the delegate didn’t display a message, so other web views should check again.

case handled

A result that indicates the delegate displayed the first use message.

case showDefault

A result that indicates the delegate didn’t display a message, so the web view should show the default Lockdown Mode message.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Displaying UI panels

func webView(WKWebView, runJavaScriptAlertPanelWithMessage: String, initiatedByFrame: WKFrameInfo, completionHandler: () -> Void)

Displays a JavaScript alert panel.

func webView(WKWebView, runJavaScriptConfirmPanelWithMessage: String, initiatedByFrame: WKFrameInfo, completionHandler: (Bool) -> Void)

Displays a JavaScript confirm panel.

func webView(WKWebView, runJavaScriptTextInputPanelWithPrompt: String, defaultText: String?, initiatedByFrame: WKFrameInfo, completionHandler: (String?) -> Void)

Displays a JavaScript text input panel.

func webView(WKWebView, showLockdownModeFirstUseMessage: String, completionHandler: (WKDialogResult) -> Void)

Displays a custom Lockdown Mode first use message.

