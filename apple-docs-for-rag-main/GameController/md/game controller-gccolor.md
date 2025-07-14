

- Game Controller
-  GCColor 

Class

# GCColor

The color of a device light.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class GCColor
```

## Topics

### Creating colors

init(red: Float, green: Float, blue: Float)

Creates a color with the specified red, green, and blue values.

### Setting color values

var red: Float

The normalized value of the red component ranging from 0 to 1.

var green: Float

The normalized value of the green component ranging from 0 to 1.

var blue: Float

The normalized value of the blue component ranging from 0 to 1.

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

### Getting the light’s color

var color: GCColor

The color of a device’s light.

