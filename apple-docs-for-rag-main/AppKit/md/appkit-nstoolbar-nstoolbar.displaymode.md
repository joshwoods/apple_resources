

- AppKit
- NSToolbar
-  NSToolbar.DisplayMode 

Enumeration

# NSToolbar.DisplayMode

Constants that indicate whether the toolbar displays items using a name, icon, or combination of elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
enum DisplayMode
```

## Topics

### Display modes

case `default`

The default display mode.

case iconAndLabel

The toolbar displays an icon and label for each item.

case iconOnly

The toolbar displays only an icon for each item.

case labelOnly

The toolbar displays only a label for each item.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the toolbar’s behavior

var isVisible: Bool

A Boolean value that indicates whether the toolbar is visible.

var displayMode: NSToolbar.DisplayMode

A value that indicates whether the toolbar displays items using a name, icon, or combination of elements.

var showsBaselineSeparator: Bool

A Boolean value that indicates whether the toolbar shows the separator between the toolbar and the main window contents.

Deprecated

var allowsUserCustomization: Bool

A Boolean value that indicates whether users can modify the contents of the toolbar.

var allowsExtensionItems: Bool

A Boolean value that indicates whether the toolbar can add items for Action extensions.

