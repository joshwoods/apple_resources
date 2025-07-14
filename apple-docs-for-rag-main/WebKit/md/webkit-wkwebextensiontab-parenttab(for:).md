

- WebKit
- WKWebExtensionTab
-  parentTab(for:) 

Instance Method

# parentTab(for:)

Called when the parent tab for the tab is needed.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func parentTab(for context: WKWebExtensionContext) -> (any WKWebExtensionTab)?
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

Defaults to `nil` if not implemented.

## See Also

### Related Documentation

func setParentTab((any WKWebExtensionTab)?, for: WKWebExtensionContext, completionHandler: ((any Error)?) -> Void)

Called to set or clear the parent tab for the tab.

