

- WebKit
- WKWebExtensionTab
-  setReaderModeActive(\_:for:completionHandler:) 

Instance Method

# setReaderModeActive(\_:for:completionHandler:)

Called to set the reader mode for the tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func setReaderModeActive(
    _ active: Bool,
    for context: WKWebExtensionContext,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
optional func setReaderModeActive(
    _ active: Bool,
    for context: WKWebExtensionContext
) async throws
```

## Parameters 

`active`  

A boolean value indicating whether to activate reader mode.

`context`  

The context in which the web extension is running.

`completionHandler`  

A block that must be called upon completion. It takes a single error argument, which should be provided if any errors occurred.

## Discussion

No action is performed if not implemented.

## See Also

### Related Documentation

func isReaderModeAvailable(for: WKWebExtensionContext) -> Bool

Called to check if reader mode is available for the tab.

func isReaderModeActive(for: WKWebExtensionContext) -> Bool

Called to check if the tab is currently showing reader mode.

