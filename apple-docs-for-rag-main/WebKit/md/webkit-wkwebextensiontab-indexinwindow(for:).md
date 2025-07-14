

- WebKit
- WKWebExtensionTab
-  indexInWindow(for:) 

Instance Method

# indexInWindow(for:)

Called when the index of the tab in the window is needed.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func indexInWindow(for context: WKWebExtensionContext) -> Int
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

This method should be implemented for better performance. Defaults to the window’s tabs(for:) method to find the index if not implemented.

