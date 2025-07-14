

- WebKit
- WKWebExtensionContext
-  didOpenTab(\_:) 

Instance Method

# didOpenTab(\_:)

Called by the app when a new tab is opened to fire appropriate events with only this extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func didOpenTab(_ newTab: any WKWebExtensionTab)
```

## Parameters 

`newTab`  

The newly opened tab.

## Discussion

This method informs only the specific extension of the opening of a new tab. If the intention is to inform all loaded extensions consistently, you should use the respective method on the extension controller instead.

## See Also

### Related Documentation

var openTabs: Set&lt;AnyHashable>

A set of open tabs in all open windows that are exposed to this extension.

