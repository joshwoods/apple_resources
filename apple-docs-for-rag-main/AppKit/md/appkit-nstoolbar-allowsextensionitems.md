

- AppKit
- NSToolbar
-  allowsExtensionItems 

Instance Property

# allowsExtensionItems

A Boolean value that indicates whether the toolbar can add items for Action extensions.

macOS 10.10+

``` source
@MainActor
var allowsExtensionItems: Bool { get set }
```

## Discussion

If the value of this property is true, the toolbar can dynamically create toolbar items for Action extensions in the toolbar configuration panel. The toolbar can only add an Action extension if its `Info.plist` file contains the NSExtensionServiceAllowsToolbarItem key with the value true. The default value of this property is false.

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

var allowsUserCustomization: Bool

A Boolean value that indicates whether users can modify the contents of the toolbar.

