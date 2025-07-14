

- WebKit
- WKWebExtensionContext
-  action(for:) 

Instance Method

# action(for:)

Retrieves the extension action for a given tab, or the default action if `nil` is passed.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func action(for tab: (any WKWebExtensionTab)?) -> WKWebExtension.Action?
```

## Parameters 

`tab`  

The tab for which to retrieve the extension action, or `nil` to get the default action.

## Discussion

The returned object represents the action specific to the tab when provided; otherwise, it returns the default action. The default action is useful when the context is unrelated to a specific tab. When possible, specify the tab to get the most context-relevant action.

## See Also

### Related Documentation

func performAction(for: (any WKWebExtensionTab)?)

Performs the extension action associated with the specified tab or performs the default action if `nil` is passed.

