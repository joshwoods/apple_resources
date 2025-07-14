

- WebKit
- WKWebExtensionTab
-  zoomFactor(for:) 

Instance Method

# zoomFactor(for:)

Called when the zoom factor of the tab is needed.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func zoomFactor(for context: WKWebExtensionContext) -> Double
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

Defaults to pageZoom of the tab’s web view if not implemented.

## See Also

### Related Documentation

func setZoomFactor(Double, for: WKWebExtensionContext, completionHandler: ((any Error)?) -> Void)

Called to set the zoom factor of the tab.

