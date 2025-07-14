

- AppKit
- NSToolbar
-  isVisible 

Instance Property

# isVisible

A Boolean value that indicates whether the toolbar is visible.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var isVisible: Bool { get set }
```

## Discussion

If the value of this property is true, the toolbar is visible; otherwise, it’s false. Change the value to hide or show the toolbar.

## See Also

### Configuring the toolbar’s behavior

var displayMode: NSToolbar.DisplayMode

A value that indicates whether the toolbar displays items using a name, icon, or combination of elements.

enum DisplayMode

Constants that indicate whether the toolbar displays items using a name, icon, or combination of elements.

var showsBaselineSeparator: Bool

A Boolean value that indicates whether the toolbar shows the separator between the toolbar and the main window contents.

Deprecated

var allowsUserCustomization: Bool

A Boolean value that indicates whether users can modify the contents of the toolbar.

var allowsExtensionItems: Bool

A Boolean value that indicates whether the toolbar can add items for Action extensions.

