

- WebKit
- WKWebExtensionTab
-  activate(for:completionHandler:) 

Instance Method

# activate(for:completionHandler:)

Called to activate the tab, making it frontmost.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func activate(
    for context: WKWebExtensionContext,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
optional func activate(for context: WKWebExtensionContext) async throws
```

## Parameters 

`context`  

The context in which the web extension is running.

`completionHandler`  

A block that must be called upon completion. It takes a single error argument, which should be provided if any errors occurred.

## Discussion

Upon activation, the tab should become the frontmost and either be the sole selected tab or be included among the selected tabs. No action is performed if not implemented.

## See Also

### Related Documentation

func setSelected(Bool, for: WKWebExtensionContext, completionHandler: ((any Error)?) -> Void)

Called to set the selected state of the tab.

