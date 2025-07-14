

- WebKit
- WKWebExtensionControllerDelegate
-  webExtensionController(\_:openOptionsPageFor:completionHandler:) 

Instance Method

# webExtensionController(\_:openOptionsPageFor:completionHandler:)

Called when an extension context requests its options page to be opened.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func webExtensionController(
    _ controller: WKWebExtensionController,
    openOptionsPageFor extensionContext: WKWebExtensionContext,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
optional func webExtensionController(
    _ controller: WKWebExtensionController,
    openOptionsPageFor extensionContext: WKWebExtensionContext
) async throws
```

## Parameters 

`controller`  

The web extension controller that is managing the extension.

`extensionContext`  

The context in which the web extension is running.

`completionHandler`  

A block to be called once the options page has been displayed or with an error if the page could not be shown.

## Discussion

This method should be implemented by the app to handle requests to display the extension’s options page. The app can decide how and where to display the options page (e.g., in a new tab or a separate window). The app should call the completion handler once the options page is visible to the user, or with an error if the operation was declined or failed. If not implemented, the options page will be opened in a new tab using the webExtensionController(_:openNewTabUsing:for:completionHandler:) delegate method.

