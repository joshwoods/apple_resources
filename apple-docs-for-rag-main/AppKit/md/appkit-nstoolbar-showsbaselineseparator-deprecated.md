

- AppKit
- NSToolbar
-  showsBaselineSeparator Deprecated

Instance Property

# showsBaselineSeparator

A Boolean value that indicates whether the toolbar shows the separator between the toolbar and the main window contents.

macOS 10.0–15.0Deprecated

``` source
@MainActor
var showsBaselineSeparator: Bool { get set }
```

Deprecated

No longer supported

## Discussion

If the value of this property is true, the toolbar shows the separator between the toolbar and the main window contents. If the value is false, the toolbar doesn’t show the separator. The default value is false.

## See Also

### Configuring the toolbar’s behavior

var isVisible: Bool

A Boolean value that indicates whether the toolbar is visible.

var displayMode: NSToolbar.DisplayMode

A value that indicates whether the toolbar displays items using a name, icon, or combination of elements.

enum DisplayMode

Constants that indicate whether the toolbar displays items using a name, icon, or combination of elements.

var allowsUserCustomization: Bool

A Boolean value that indicates whether users can modify the contents of the toolbar.

var allowsExtensionItems: Bool

A Boolean value that indicates whether the toolbar can add items for Action extensions.

