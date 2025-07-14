

- WebKit
- WKUIDelegate
-  webView(\_:commitPreviewingViewController:) Deprecated

Instance Method

# webView(\_:commitPreviewingViewController:)

Called when the user performs a pop action on the preview.

iOS 10.0–13.0DeprecatediPadOS 10.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    commitPreviewingViewController previewingViewController: UIViewController
)
```

## Parameters 

`webView`  

The web view invoking the delegate method.

`previewingViewController`  

The view controller that is popped.

## Discussion

You must display the previewed view controller inside of your app.

## See Also

### Responding to Force Touch actions

func webView(WKWebView, shouldPreviewElement: WKPreviewElementInfo) -> Bool

Determines whether the given element should show a preview.

Deprecated

func webView(WKWebView, previewingViewControllerForElement: WKPreviewElementInfo, defaultActions: [any WKPreviewActionItem]) -> UIViewController?

Called when the user performs a peek action.

Deprecated

