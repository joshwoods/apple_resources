

- WebKit
- WKWebExtensionTab
-  setZoomFactor(\_:for:completionHandler:) 

Instance Method

# setZoomFactor(\_:for:completionHandler:)

Called to set the zoom factor of the tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func setZoomFactor(
    _ zoomFactor: Double,
    for context: WKWebExtensionContext,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
optional func setZoomFactor(
    _ zoomFactor: Double,
    for context: WKWebExtensionContext
) async throws
```

## Parameters 

`zoomFactor`  

The desired zoom factor for the tab.

`context`  

The context in which the web extension is running.

`completionHandler`  

A block that must be called upon completion. It takes a single error argument, which should be provided if any errors occurred.

## Discussion

Sets pageZoom of the tab’s web view if not implemented.

## See Also

### Related Documentation

func zoomFactor(for: WKWebExtensionContext) -> Double

Called when the zoom factor of the tab is needed.

