

- WebKit
- WKWebExtensionTab
-  reload(fromOrigin:for:completionHandler:) 

Instance Method

# reload(fromOrigin:for:completionHandler:)

Called to reload the current page in the tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func reload(
    fromOrigin: Bool,
    for context: WKWebExtensionContext,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
optional func reload(
    fromOrigin: Bool,
    for context: WKWebExtensionContext
) async throws
```

## Parameters 

`fromOrigin`  

A boolean value indicating whether to reload the tab from the origin, bypassing the cache.

`context`  

The context in which the web extension is running.

`completionHandler`  

A block that must be called upon completion. It takes a single error argument, which should be provided if any errors occurred.

## Discussion

Reloads the tab’s web view via reload() or reloadFromOrigin() if not implemented.

