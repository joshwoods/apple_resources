

- UIKit
-  UITitlebarSeparatorStyle 

Enumeration

# UITitlebarSeparatorStyle

Styles that determine the type of separator displayed between the title bar and content of a window.

Mac Catalyst 14.0+

``` source
enum UITitlebarSeparatorStyle
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

### Configuring the title bar

var separatorStyle: UITitlebarSeparatorStyle

The type of separator that the app displays between the title bar and content of a window.

var titleVisibility: UITitlebarTitleVisibility

A value that indicates the visibility of the title.

enum UITitlebarTitleVisibility

States that determine visibility of the title in the title bar.

var representedURL: URL?

A URL of the file or resource represented in the window.

