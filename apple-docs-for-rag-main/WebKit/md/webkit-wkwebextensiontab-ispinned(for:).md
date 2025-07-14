

- WebKit
- WKWebExtensionTab
-  isPinned(for:) 

Instance Method

# isPinned(for:)

Called when the pinned state of the tab is needed.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func isPinned(for context: WKWebExtensionContext) -> Bool
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

Defaults to `NO` if not implemented.

## See Also

### Related Documentation

func setPinned(Bool, for: WKWebExtensionContext, completionHandler: ((any Error)?) -> Void)

Called to set the pinned state of the tab.

