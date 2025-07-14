

- UIKit
- UITableViewRowAction
-  UITableViewRowAction.Style Deprecated

Enumeration

# UITableViewRowAction.Style

Constants that specify the appearance of action buttons.

iOS 8.0–13.0DeprecatediPadOS 8.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
enum Style
```

## Topics

### Styles

case `default`

Apply the default style to the button.

static var destructive: UITableViewRowAction.Style

Equal to the default style.

case normal

Apply a style that reflects standard non-destructive actions.

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

### Configuring the action’s appearance

var style: UITableViewRowAction.Style

The style applied to the action button.

Deprecated

var title: String?

The title of the action button.

Deprecated

var backgroundColor: UIColor?

The background color of the action button.

Deprecated

var backgroundEffect: UIVisualEffect?

The visual effect to apply to the button.

Deprecated

