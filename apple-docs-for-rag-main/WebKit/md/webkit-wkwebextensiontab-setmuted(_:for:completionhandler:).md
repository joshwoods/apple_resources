

- WebKit
- WKWebExtensionTab
-  setMuted(\_:for:completionHandler:) 

Instance Method

# setMuted(\_:for:completionHandler:)

Called to set the mute state of the tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func setMuted(
    _ muted: Bool,
    for context: WKWebExtensionContext,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
optional func setMuted(
    _ muted: Bool,
    for context: WKWebExtensionContext
) async throws
```

## Parameters 

`muted`  

A boolean indicating whether the tab should be muted.

`context`  

The context in which the web extension is running.

`completionHandler`  

A block that must be called upon completion. It takes a single error argument, which should be provided if any errors occurred.

## Discussion

No action is performed if not implemented.

## See Also

### Related Documentation

func isMuted(for: WKWebExtensionContext) -> Bool

Called to check if the tab is currently muted.

