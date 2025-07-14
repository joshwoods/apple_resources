

- WebKit
- WKWebExtensionControllerDelegate
-  webExtensionController(\_:presentActionPopup:for:completionHandler:) 

Instance Method

# webExtensionController(\_:presentActionPopup:for:completionHandler:)

Called when a popup is requested to be displayed for a specific action.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func webExtensionController(
    _ controller: WKWebExtensionController,
    presentActionPopup action: WKWebExtension.Action,
    for context: WKWebExtensionContext,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
optional func webExtensionController(
    _ controller: WKWebExtensionController,
    presentActionPopup action: WKWebExtension.Action,
    for context: WKWebExtensionContext
) async throws
```

## Parameters 

`controller`  

The web extension controller initiating the request.

`action`  

The action for which the popup is requested.

`context`  

The context within which the web extension is running.

`completionHandler`  

A block to be called once the popup display operation is completed.

## Discussion

This method is called in response to the extension’s scripts or when invoking performAction(for:) if the action has a popup.

The associated tab, if applicable, can be located through the associatedTab property of the `action` parameter. This delegate method is called when the web view for the popup is fully loaded and ready to display. Implementing this method is needed if the app intends to support programmatically showing the popup by the extension, although it is recommended for handling both programmatic and user-initiated cases.

