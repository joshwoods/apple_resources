

- WebKit
- WKUIDelegate
-  webView(\_:contextMenuConfigurationForElement:completionHandler:) 

Instance Method

# webView(\_:contextMenuConfigurationForElement:completionHandler:)

Tells the delegate that a contextual menu interaction began.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    contextMenuConfigurationForElement elementInfo: WKContextMenuElementInfo,
    completionHandler: @escaping @MainActor (UIContextMenuConfiguration?) -> Void
)
```

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    contextMenuConfigurationFor elementInfo: WKContextMenuElementInfo
) async -> UIContextMenuConfiguration?
```

## Parameters 

`webView`  

The web view in which the interaction occurred.

`elementInfo`  

An object that contains information about the element involved in the interaction.

`completionHandler`  

The completion handler for you to call with information about how you want to handle the interaction. This handler block has no return value and takes the following parameter:

configuration  
The UIContextMenuConfiguration object that contains the details of how you want to handle the interaction. Specify `nil` for this parameter if you don’t want to show a contextual menu.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func webView(_ webView: WKWebView, contextMenuConfigurationFor elementInfo: WKContextMenuElementInfo) async -> UIContextMenuConfiguration?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Displaying a contextual menu

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

func webView(WKWebView, contextMenuForElement: WKContextMenuElementInfo, willCommitWithAnimator: any UIContextMenuInteractionCommitAnimating)

Provides the delegate with the animator object that the web view uses to display the contextual menu.

func webView(WKWebView, contextMenuWillPresentForElement: WKContextMenuElementInfo)

Tells the delegate that the web view is about to present the contextual menu for the specified element.

func webView(WKWebView, contextMenuDidEndForElement: WKContextMenuElementInfo)

Tells the delegate that the web view dismissed the contextual menu for the specified element.

@MainActor class UIContextMenuConfiguration

An object containing the configuration details for the contextual menu.

