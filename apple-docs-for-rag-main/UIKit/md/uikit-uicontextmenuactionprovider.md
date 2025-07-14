

- UIKit
-  UIContextMenuActionProvider 

Type Alias

# UIContextMenuActionProvider

Returns an action-based contextual menu, optionally incorporating the system-suggested actions.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
typealias UIContextMenuActionProvider = ([UIMenuElement]) -> UIMenu?
```

## Parameters 

`suggestedActions`  

Suggested actions for you to include in your menu. UIKit collects these actions from responders in the current responder chain. You are not required to include the actions in your menu.

## Return Value

The menu object containing the actions for the user to select.

## Discussion

Use this handler to create UIAction objects representing the actions the user may choose from your menu. To organize groups of actions hierarchically, create a UIMenu object to represent a submenu and add nested actions to it. Finally, build your top-level UIMenu object from the actions and submenus you created, and return that menu object from your handler.

## See Also

### Creating the menu configuration object

convenience init(identifier: (any NSCopying)?, previewProvider: UIContextMenuContentPreviewProvider?, actionProvider: UIContextMenuActionProvider?)

Creates a menu configuration object with the specified action and preview providers.

typealias UIContextMenuContentPreviewProvider

Returns the custom view controller to use when previewing your content.

