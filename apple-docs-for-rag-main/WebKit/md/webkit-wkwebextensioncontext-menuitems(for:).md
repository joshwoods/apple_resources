

- WebKit
- WKWebExtensionContext
-  menuItems(for:) 

Instance Method

# menuItems(for:)

Retrieves the menu items for a given tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

**macOS**

``` source
@MainActor
func menuItems(for tab: any WKWebExtensionTab) -> [NSMenuItem]
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
@MainActor
func menuItems(for tab: any WKWebExtensionTab) -> [UIMenuElement]
```

## Parameters 

`tab`  

The tab for which to retrieve the menu items.

## Discussion

Returns menu items provided by the extension, allowing the user to perform extension-defined actions on the tab.

The app is responsible for displaying these menu items, typically in a context menu or a long-press menu on the tab.

Note

The properties of the menu items, including the items themselves, can change dynamically. Therefore, the app should fetch the menu items immediately before showing them, to ensure that the most current and relevant items are presented.

