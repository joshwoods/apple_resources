

- MetricKit
-  MXUnitAveragePixelLuminance 

Class

# MXUnitAveragePixelLuminance

A unit of measure of pixel luminosity on an OLED display.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXUnitAveragePixelLuminance
```

## Overview

Luminosity represents the brightness of each red, green, and blue component pixel. Unlike LCD displays, each pixel requires power to display a color, and white draws the most power per pixel.

`MXUnitAveragePixelLuminance` defines the base unit as the average luminance of all the pixels on the screen for some period of time. Reducing the average luminance of the display reduces the amount of power consumed by the app.

## Topics

### Measuring Average Pixel Luminance

class var apl: MXUnitAveragePixelLuminance

The average number of powered pixels on a OLED display.

## Relationships

### Inherits From

- Dimension

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
- Sendable

## See Also

### Reading average active pixel use

var averagePixelLuminance: MXAverage&lt;MXUnitAveragePixelLuminance>?

The average amount of luminosity of the pixels on an OLED display.

