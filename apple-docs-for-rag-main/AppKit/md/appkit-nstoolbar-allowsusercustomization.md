

- AppKit
- NSToolbar
-  allowsUserCustomization 

Instance Property

# allowsUserCustomization

A Boolean value that indicates whether users can modify the contents of the toolbar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var allowsUserCustomization: Bool { get set }
```

## Discussion

If the value of this property is true, the toolbar enables the Customize Toolbar… menu item. If the value is false, the toolbar disables this menu item. The Customize Toolbar… menu item lets people change the items on the toolbar, rearrange their positions, and change the toolbar’s display mode. This attribute does not affect someone’s ability to show or hide the toolbar. The default value of this property is false.

You can change the value of this property at any time to change your toolbar’s customization behavior. For example, you might prevent toolbar customizations while your app processes some other event. If you set this property to true, set the autosavesConfiguration property to true to persist any customizations.

## See Also

### Configuring the toolbar’s behavior

var isVisible: Bool

A Boolean value that indicates whether the toolbar is visible.

var displayMode: NSToolbar.DisplayMode

A value that indicates whether the toolbar displays items using a name, icon, or combination of elements.

enum DisplayMode

Constants that indicate whether the toolbar displays items using a name, icon, or combination of elements.

var showsBaselineSeparator: Bool

A Boolean value that indicates whether the toolbar shows the separator between the toolbar and the main window contents.

Deprecated

var allowsExtensionItems: Bool

A Boolean value that indicates whether the toolbar can add items for Action extensions.

