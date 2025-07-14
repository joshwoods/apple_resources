

- WebKit
- WKWebExtensionTab
-  setPinned(\_:for:completionHandler:) 

Instance Method

# setPinned(\_:for:completionHandler:)

Called to set the pinned state of the tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func setPinned(
    _ pinned: Bool,
    for context: WKWebExtensionContext,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
optional func setPinned(
    _ pinned: Bool,
    for context: WKWebExtensionContext
) async throws
```

## Parameters 

`pinned`  

A boolean value indicating whether to pin the tab.

`context`  

The context in which the web extension is running.

`completionHandler`  

A block that must be called upon completion. It takes a single error argument, which should be provided if any errors occurred.

## Discussion

This is equivalent to the user selecting to pin or unpin the tab through a menu item. When a tab is pinned, it should be moved to the front of the tab bar and usually reduced in size. When a tab is unpinned, it should be restored to a normal size and position in the tab bar. No action is performed if not implemented.

## See Also

### Related Documentation

func isPinned(for: WKWebExtensionContext) -> Bool

Called when the pinned state of the tab is needed.

