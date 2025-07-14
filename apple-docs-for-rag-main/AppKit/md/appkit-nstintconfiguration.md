

- AppKit
-  NSTintConfiguration 

Class

# NSTintConfiguration

An object that gives you the ability to choose from system-provided tinting behaviors.

macOS 11.0+

``` source
class NSTintConfiguration
```

## Topics

### Initializing a Tint Configuration

convenience init(fixedColor: NSColor)

Creates a new tint configuration using a specific color value.

convenience init(preferredColor: NSColor)

Creates a new tint configuration for the system to use when the app’s preferred accent color is in use.

### Changing an App’s Appearance

var adaptsToUserAccentColor: Bool

A Boolean value that indicates whether the tint configuration alters its effect based on the user’s preferred accent color choice.

### Setting the Tint Color

class var `default`: NSTintConfiguration

The system tints the content using the system default value for its context.

class var monochrome: NSTintConfiguration

The content always displays in monochrome.

var baseTintColor: NSColor?

The color the system supplies when you create a tint configuration.

var equivalentContentTintColor: NSColor?

A color object that matches the effective content tint.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Customizing Tint Color

func outlineView(NSOutlineView, tintConfigurationForItem: Any) -> NSTintConfiguration?

Customizes an item’s tinting behavior.

