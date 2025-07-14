

- UIKit
- UIBarButtonItem
-  UIBarButtonItem.Style 

Enumeration

# UIBarButtonItem.Style

Constants that specify the style of an item.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum Style
```

## Topics

### Constants

case plain

A button style with plain text styling.

case bordered

A simple button style with a border.

case done

A button style for a done button.

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

### Customizing item appearance

var style: UIBarButtonItem.Style

The style of the item.

var tintColor: UIColor?

The tint color to apply to the button item.

var isHidden: Bool

A Boolean that determines the visibility of the item.

var isSelected: Bool

A Boolean value that indicates whether the button is in a selected state.

var width: CGFloat

The width of the item.

var possibleTitles: Set&lt;String>?

The set of possible titles to display on the bar button.

