

- WebKit
- WKWebExtensionTab
-  setParentTab(\_:for:completionHandler:) 

Instance Method

# setParentTab(\_:for:completionHandler:)

Called to set or clear the parent tab for the tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func setParentTab(
    _ parentTab: (any WKWebExtensionTab)?,
    for context: WKWebExtensionContext,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
optional func setParentTab(
    _ parentTab: (any WKWebExtensionTab)?,
    for context: WKWebExtensionContext
) async throws
```

## Parameters 

`parentTab`  

The tab that should be set as the parent of the tab. If \c nil is provided, the current parent tab should be cleared.

`context`  

The context in which the web extension is running.

`completionHandler`  

A block that must be called upon completion. It takes a single error argument, which should be provided if any errors occurred.

## Discussion

No action is performed if not implemented.

## See Also

### Related Documentation

func parentTab(for: WKWebExtensionContext) -> (any WKWebExtensionTab)?

Called when the parent tab for the tab is needed.

