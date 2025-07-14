

- WebKit
- WKWebExtensionController
-  didSelectTabs(\_:) 

Instance Method

# didSelectTabs(\_:)

Should be called by the app when tabs are selected to fire appropriate events with all loaded web extensions.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func didSelectTabs(_ selectedTabs: [any WKWebExtensionTab])
```

## Parameters 

`selectedTabs`  

The set of tabs that were selected.

## Discussion

This method informs all loaded extensions that tabs have been selected, ensuring consistent understanding across extensions.

If the intention is to inform only a specific extension, you should use the respective method on that extension’s context instead.

