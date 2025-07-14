

- AppKit
- NSSliderCell
-  maxValue 

Instance Property

# maxValue

The maximum value the slider can send to its target.

macOS

``` source
@MainActor
var maxValue: Double { get set }
```

## Discussion

A horizontal slider sends its maximum value when the knob is at the right end of the slider; a vertical slider sends it when the knob is at the top. The maximum selectable value for a circular slider is just below maxValue; for example, if maxValue is 360, you can set the dial up to 359.999.

## See Also

### Managing Value Limits

var minValue: Double

The minimum value the slider can send to its target.

