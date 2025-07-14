

- AppKit
- NSMenu
-  NSMenu.PresentationStyle 

Enumeration

# NSMenu.PresentationStyle

Specifies the style of a menu.

macOS 14.0+

``` source
enum PresentationStyle
```

## Topics

### Defining the menu style

case palette

A menu presentation style where items to display align horizontally.

case regular

The default presentation style for a menu.

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

### Managing Presentation Styles

var presentationStyle: NSMenu.PresentationStyle

The presentation style of the menu.

