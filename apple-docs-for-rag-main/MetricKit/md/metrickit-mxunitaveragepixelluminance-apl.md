

- MetricKit
- MXUnitAveragePixelLuminance
-  apl 

Type Property

# apl

The average number of powered pixels on a OLED display.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@NSCopying
class var apl: MXUnitAveragePixelLuminance { get }
```

## Discussion

The value of `apl` is a whole number ranging from 0 to 100. 0 means the display is black with no illuminated pixels. A value of 100 means the display is white with all red, green, and blue components of all pixels illuminated.

