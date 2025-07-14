

- WebKit
- WKUIDelegate
-  Deprecated symbols 

API Collection

# Deprecated symbols

Review unsupported symbols and their replacements.

## Topics

### Responding to Force Touch actions

func webView(WKWebView, shouldPreviewElement: WKPreviewElementInfo) -> Bool

Determines whether the given element should show a preview.

Deprecated

func webView(WKWebView, previewingViewControllerForElement: WKPreviewElementInfo, defaultActions: [any WKPreviewActionItem]) -> UIViewController?

Called when the user performs a peek action.

Deprecated

func webView(WKWebView, commitPreviewingViewController: UIViewController)

Called when the user performs a pop action on the preview.

Deprecated

