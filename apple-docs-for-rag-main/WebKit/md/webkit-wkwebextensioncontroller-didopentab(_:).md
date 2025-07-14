

- WebKit
- WKWebExtensionController
-  didOpenTab(\_:) 

Instance Method

# didOpenTab(\_:)

Should be called by the app when a new tab is opened to fire appropriate events with all loaded web extensions.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func didOpenTab(_ newTab: any WKWebExtensionTab)
```

## Parameters 

`newTab`  

The newly opened tab.

## Discussion

This method informs all loaded extensions of the opening of a new tab, ensuring consistent understanding across extensions.

If the intention is to inform only a specific extension, you should use the respective method on that extension’s context instead.

## See Also

### Related Documentation

func didCloseTab(any WKWebExtensionTab, windowIsClosing: Bool)

Should be called by the app when a tab is closed to fire appropriate events with all loaded web extensions.

