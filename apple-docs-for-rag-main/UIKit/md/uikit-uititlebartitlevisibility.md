

- UIKit
-  UITitlebarTitleVisibility 

Enumeration

# UITitlebarTitleVisibility

States that determine visibility of the title in the title bar.

Mac Catalyst 13.0+

``` source
enum UITitlebarTitleVisibility
```

## Topics

### Visibility states

case visible

A state indicating that the title is visible in the title bar.

case hidden

A state indicating that the title isn’t visible in the title bar.

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

enum UITitlebarSeparatorStyle

Styles that determine the type of separator displayed between the title bar and content of a window.

var titleVisibility: UITitlebarTitleVisibility

A value that indicates the visibility of the title.

var representedURL: URL?

A URL of the file or resource represented in the window.

