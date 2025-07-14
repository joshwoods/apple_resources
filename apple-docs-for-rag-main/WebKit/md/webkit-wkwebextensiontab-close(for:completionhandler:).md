

- WebKit
- WKWebExtensionTab
-  close(for:completionHandler:) 

Instance Method

# close(for:completionHandler:)

Called to close the tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func close(
    for context: WKWebExtensionContext,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
optional func close(for context: WKWebExtensionContext) async throws
```

## Parameters 

`context`  

The context in which the web extension is running.

`completionHandler`  

A block that must be called upon completion. It takes a single error argument, which should be provided if any errors occurred.

## Discussion

No action is performed if not implemented.

