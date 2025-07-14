

- AppKit
- NSSliderCell
-  minValue 

Instance Property

# minValue

The minimum value the slider can send to its target.

macOS

``` source
@MainActor
var minValue: Double { get set }
```

## Discussion

A vertical slider sends this value when its knob is at the bottom; a horizontal slider sends it when its knob is all the way to the left; a circular slider sends it when its knob is at the top.

## See Also

### Managing Value Limits

var maxValue: Double

The maximum value the slider can send to its target.

