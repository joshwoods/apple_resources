

- WebKit
- WKUIDelegate
-  webView(\_:contextMenuDidEndForElement:) 

Instance Method

# webView(\_:contextMenuDidEndForElement:)

Tells the delegate that the web view dismissed the contextual menu for the specified element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    contextMenuDidEndForElement elementInfo: WKContextMenuElementInfo
)
```

## Parameters 

`webView`  

The web view in which the interaction occurred.

`elementInfo`  

An object that contains information about the element involved in the interaction.

## See Also

### Displaying a contextual menu

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

func webView(WKWebView, contextMenuConfigurationForElement: WKContextMenuElementInfo, completionHandler: (UIContextMenuConfiguration?) -> Void)

Tells the delegate that a contextual menu interaction began.

func webView(WKWebView, contextMenuForElement: WKContextMenuElementInfo, willCommitWithAnimator: any UIContextMenuInteractionCommitAnimating)

Provides the delegate with the animator object that the web view uses to display the contextual menu.

func webView(WKWebView, contextMenuWillPresentForElement: WKContextMenuElementInfo)

Tells the delegate that the web view is about to present the contextual menu for the specified element.

@MainActor class UIContextMenuConfiguration

An object containing the configuration details for the contextual menu.

