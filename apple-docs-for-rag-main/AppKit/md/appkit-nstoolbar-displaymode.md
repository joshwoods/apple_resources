

- AppKit
- NSToolbar
-  displayMode 

Instance Property

# displayMode

A value that indicates whether the toolbar displays items using a name, icon, or combination of elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var displayMode: NSToolbar.DisplayMode { get set }
```

## Discussion

The default value of this property is NSToolbar.DisplayMode.default. For a list of possible values, see NSToolbar.DisplayMode.

## See Also

### Configuring the toolbar’s behavior

var isVisible: Bool

A Boolean value that indicates whether the toolbar is visible.

enum DisplayMode

Constants that indicate whether the toolbar displays items using a name, icon, or combination of elements.

var showsBaselineSeparator: Bool

A Boolean value that indicates whether the toolbar shows the separator between the toolbar and the main window contents.

Deprecated

var allowsUserCustomization: Bool

A Boolean value that indicates whether users can modify the contents of the toolbar.

var allowsExtensionItems: Bool

A Boolean value that indicates whether the toolbar can add items for Action extensions.

