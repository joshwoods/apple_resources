

- AppKit
- NSComboButton
-  NSComboButton.Style 

Enumeration

# NSComboButton.Style

Constants that indicate how a combo button presents its menu.

macOS 13.0+

``` source
enum Style
```

## Topics

### Getting the Combo Button Styles

case split

A style that separates the button’s title and image from the menu indicator people use to activate the button.

case unified

A style that unifies the button’s title and image with the menu indicator.

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

### Configuring the Button Appearance

var style: NSComboButton.Style

The appearance setting that determines how the button presents its menu .

var title: String

The localized string that the button displays.

var image: NSImage?

The image that the button displays.

var imageScaling: NSImageScaling

The scaling behavior to apply to the button’s image.

