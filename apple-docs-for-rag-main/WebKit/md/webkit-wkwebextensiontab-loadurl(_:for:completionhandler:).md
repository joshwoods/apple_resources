

- WebKit
- WKWebExtensionTab
-  loadURL(\_:for:completionHandler:) 

Instance Method

# loadURL(\_:for:completionHandler:)

Called to load a URL in the tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func loadURL(
    _ url: URL,
    for context: WKWebExtensionContext,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
optional func loadURL(
    _ url: URL,
    for context: WKWebExtensionContext
) async throws
```

## Parameters 

`url`  

The URL to be loaded in the tab.

`context`  

The context in which the web extension is running.

`completionHandler`  

A block that must be called upon completion. It takes a single error argument, which should be provided if any errors occurred.

## Discussion

If the tab is already loading a page, calling this method should stop the current page from loading and start loading the new URL. Loads the URL in the tab’s web view via load(_:) if not implemented.

