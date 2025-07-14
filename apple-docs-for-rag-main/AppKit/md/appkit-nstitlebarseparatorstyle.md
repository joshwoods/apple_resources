

- AppKit
-  NSTitlebarSeparatorStyle 

Enumeration

# NSTitlebarSeparatorStyle

Styles that determine the type of separator displayed between the title bar and content of a window.

macOS 11.0+

``` source
enum NSTitlebarSeparatorStyle
```

## Topics

### Styles

case automatic

A style indicating that the system determines the type of separator.

case line

A style indicating that the title bar separator is a line.

case none

A style indicating that there’s no title bar separator.

case shadow

A style indicating that the title bar separator is a shadow.

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

### Customizing Appearance

var allowsFullHeightLayout: Bool

A Boolean value that indicates whether full-height sidebars appear in the window after you set a style mask.

var titlebarSeparatorStyle: NSTitlebarSeparatorStyle

The type of separator that the app displays between the title bar and content of a window.

