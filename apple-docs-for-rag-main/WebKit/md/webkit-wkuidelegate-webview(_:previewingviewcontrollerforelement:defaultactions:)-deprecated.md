

- WebKit
- WKUIDelegate
-  webView(\_:previewingViewControllerForElement:defaultActions:) Deprecated

Instance Method

# webView(\_:previewingViewControllerForElement:defaultActions:)

Called when the user performs a peek action.

iOS 10.0–13.0DeprecatediPadOS 10.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    previewingViewControllerForElement elementInfo: WKPreviewElementInfo,
    defaultActions previewActions: [any WKPreviewActionItem]
) -> UIViewController?
```

## Parameters 

`webView`  

The web view invoking the delegate method.

`elementInfo`  

The information associated with the element.

`previewActions`  

An array of default actions used by the element.

## Return Value

Return `nil` to use Webkit’s default preview behavior. Returning a view controller allows webView(_:commitPreviewingViewController:) to be invoked when the user performs a pop action.

## Discussion

To use the default actions, your app must return the actions to be run in your view controller’s implementation of previewActionItems.

## See Also

### Responding to Force Touch actions

func webView(WKWebView, shouldPreviewElement: WKPreviewElementInfo) -> Bool

Determines whether the given element should show a preview.

Deprecated

func webView(WKWebView, commitPreviewingViewController: UIViewController)

Called when the user performs a pop action on the preview.

Deprecated

