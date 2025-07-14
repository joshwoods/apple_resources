

- WebKit
- WKWebExtensionTab
-  goForward(for:completionHandler:) 

Instance Method

# goForward(for:completionHandler:)

Called to navigate the tab to the next page in its history.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func goForward(
    for context: WKWebExtensionContext,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
optional func goForward(for context: WKWebExtensionContext) async throws
```

## Parameters 

`context`  

The context in which the web extension is running.

`completionHandler`  

A block that must be called upon completion. It takes a single error argument, which should be provided if any errors occurred.

## Discussion

Navigates to the next page in the tab’s web view via goForward() if not implemented.

