

- AppKit
-  NSColorPickerTouchBarItem 

Class

# NSColorPickerTouchBarItem

A bar item that provides a system-defined color picker.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
class NSColorPickerTouchBarItem
```

## Overview

For design guidance, see Human Interface Guidelines.

## Topics

### Creating a color picker item

class func colorPicker(withIdentifier: NSTouchBarItem.Identifier) -> Self

Creates a bar item with the standard color picker icon.

class func textColorPicker(withIdentifier: NSTouchBarItem.Identifier) -> Self

Creates a bar item with the standard text color picker icon.

class func strokeColorPicker(withIdentifier: NSTouchBarItem.Identifier) -> Self

Creates a bar item with the standard stroke color picker icon.

class func colorPicker(withIdentifier: NSTouchBarItem.Identifier, buttonImage: UIImage) -> Self

Creates a color picker bar item using the supplied image as its icon.

### Configuring the color picker

var colorList: NSColorList!

The list of colors displayed in the color picker.

var allowedColorSpaces: [NSColorSpace]?

Controls the color spaces that the color picker can produce.

var showsAlpha: Bool

A Boolean value that controls whether the color picker allows picking of colors with alpha values other than `1.0`.

var isEnabled: Bool

A Boolean value that determines whether the color picker is enabled.

### Obtaining the selected color

var color: UIColor

The picker’s currently selected color.

var target: AnyObject?

An object that is notified when a user interacts with the color picker.

var action: Selector?

The selector on the target object that is invoked when a user interacts with the color picker.

### Configuring bar customization

var customizationLabel: String!

The user-visible string identifying this item during touch bar customization.

## Relationships

### Inherits From

- NSTouchBarItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable

## See Also

### Color Selection

class NSColorPicker

An abstract superclass that implements the default color picking protocol.

class NSColorWell

A control that displays a color value and lets the user change that color value.

