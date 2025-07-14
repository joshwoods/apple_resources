

- WebKit
- WKWebExtensionControllerDelegate
-  webExtensionController(\_:promptForPermissions:in:for:completionHandler:) 

Instance Method

# webExtensionController(\_:promptForPermissions:in:for:completionHandler:)

Called when an extension context requests permissions.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func webExtensionController(
    _ controller: WKWebExtensionController,
    promptForPermissions permissions: Set,
    in tab: (any WKWebExtensionTab)?,
    for extensionContext: WKWebExtensionContext,
    completionHandler: @escaping (Set, Date?) -> Void
)
```

``` source
@MainActor
optional func webExtensionController(
    _ controller: WKWebExtensionController,
    promptForPermissions permissions: Set,
    in tab: (any WKWebExtensionTab)?,
    for extensionContext: WKWebExtensionContext
) async -> (Set, Date?)
```

## Parameters 

`controller`  

The web extension controller that is managing the extension.

`permissions`  

The set of permissions being requested by the extension.

`tab`  

The tab in which the extension is running, or \c nil if the request is not specific to a tab.

`extensionContext`  

The context in which the web extension is running.

`completionHandler`  

A block to be called with the set of allowed permissions and an optional expiration date.

## Discussion

This method should be implemented by the app to prompt the user for permission and call the completion handler with the set of permissions that were granted and an optional expiration date. If not implemented or the completion handler is not called within a reasonable amount of time, the request is assumed to have been denied. The expiration date can be used to specify when the permissions expire. If `nil`, permissions are assumed to not expire.

