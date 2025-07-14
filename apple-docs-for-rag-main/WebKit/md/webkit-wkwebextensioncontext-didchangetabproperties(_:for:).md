

- WebKit
- WKWebExtensionContext
-  didChangeTabProperties(\_:for:) 

Instance Method

# didChangeTabProperties(\_:for:)

Called by the app when the properties of a tab are changed to fire appropriate events with only this extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func didChangeTabProperties(
    _ properties: WKWebExtension.TabChangedProperties,
    for changedTab: any WKWebExtensionTab
)
```

## Parameters 

`properties`  

The properties of the tab that were changed.

`changedTab`  

The tab whose properties were changed.

## Discussion

This method informs only the specific extension of the changes to a tab’s properties. If the intention is to inform all loaded extensions consistently, you should use the respective method on the extension controller instead.

