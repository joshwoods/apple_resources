

- UIKit
-  UITitlebarToolbarStyle 

Enumeration

# UITitlebarToolbarStyle

Styles that determine the toolbar’s appearance and location related to the title bar.

Mac Catalyst 14.0+

``` source
enum UITitlebarToolbarStyle
```

## Topics

### Styles

case automatic

A style indicating that the system determines the toolbar’s appearance and location.

case expanded

A style indicating that the toolbar appears below the window title.

case preference

A style indicating that the toolbar appears below the window title with toolbar items centered in the toolbar.

case unified

A style indicating that the toolbar appears inline with the window title.

case unifiedCompact

A style indicating that the toolbar appears inline with the window title and with reduced margins to allow more focus on the window’s contents.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the toolbar

var toolbar: NSToolbar?

The toolbar displayed beneath or integrated with the title bar.

var toolbarStyle: UITitlebarToolbarStyle

The style of the toolbar determining its appearance and location related to the title bar.

var autoHidesToolbarInFullScreen: Bool

A Boolean value that determines whether the toolbar automatically hides in full-screen windows.

