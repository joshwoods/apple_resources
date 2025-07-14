

- WebKit
- WKUIDelegate
-  webView(\_:shouldPreviewElement:) Deprecated

Instance Method

# webView(\_:shouldPreviewElement:)

Determines whether the given element should show a preview.

iOS 10.0–13.0DeprecatediPadOS 10.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    shouldPreviewElement elementInfo: WKPreviewElementInfo
) -> Bool
```

## Parameters 

`webView`  

The web view invoking the delegate method.

`elementInfo`  

The information associated with the element.

## Return Value

Return `NO` to disable previews for the given element.

## Discussion

This method is only invoked for elements that have a default preview in WebKit.

## See Also

### Responding to Force Touch actions

func webView(WKWebView, previewingViewControllerForElement: WKPreviewElementInfo, defaultActions: [any WKPreviewActionItem]) -> UIViewController?

Called when the user performs a peek action.

Deprecated

func webView(WKWebView, commitPreviewingViewController: UIViewController)

Called when the user performs a pop action on the preview.

Deprecated

