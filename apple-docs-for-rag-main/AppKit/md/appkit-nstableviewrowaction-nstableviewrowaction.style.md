

- AppKit
- NSTableViewRowAction
-  NSTableViewRowAction.Style 

Enumeration

# NSTableViewRowAction.Style

Constants that help define the appearance and behavior of action buttons.

macOS 10.11+

``` source
enum Style
```

## Topics

### Constants

case regular

Apply the default style to the button. This style does not apply any special coloring to the button.

case destructive

Apply a style that indicates that the action might change or delete data. This style changes the value of the backgroundColor property to an appropriate value to reflect the destructive action. After creating the action object, you can change the background color as needed. Destructive actions require a longer swipe to activate, and trigger an animation when a table row is deleted.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

