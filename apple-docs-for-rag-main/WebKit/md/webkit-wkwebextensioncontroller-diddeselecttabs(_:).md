

- WebKit
- WKWebExtensionController
-  didDeselectTabs(\_:) 

Instance Method

# didDeselectTabs(\_:)

Should be called by the app when tabs are deselected to fire appropriate events with all loaded web extensions.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func didDeselectTabs(_ deselectedTabs: [any WKWebExtensionTab])
```

## Parameters 

`deselectedTabs`  

The set of tabs that were deselected.

## Discussion

This method informs all loaded extensions that tabs have been deselected, ensuring consistent understanding across extensions.

If the intention is to inform only a specific extension, you should use the respective method on that extension’s context instead.

