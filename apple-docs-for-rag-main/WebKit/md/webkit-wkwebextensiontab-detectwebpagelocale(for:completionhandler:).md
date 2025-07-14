

- WebKit
- WKWebExtensionTab
-  detectWebpageLocale(for:completionHandler:) 

Instance Method

# detectWebpageLocale(for:completionHandler:)

Called to detect the locale of the webpage currently loaded in the tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func detectWebpageLocale(
    for context: WKWebExtensionContext,
    completionHandler: @escaping (Locale?, (any Error)?) -> Void
)
```

``` source
@MainActor
optional func detectWebpageLocale(for context: WKWebExtensionContext) async throws -> Locale?
```

## Parameters 

`context`  

The context in which the web extension is running.

`completionHandler`  

A block that must be called upon completion. The block takes two arguments: the detected locale (or `nil` if the locale is unknown) and an error, which should be provided if any errors occurred.

## Discussion

No action is performed if not implemented.

