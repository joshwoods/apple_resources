

- AppKit
- NSSlider
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

A horizontal slider sends the minimum value when the knob is all the way to the leading end of the bar. A vertical slider sends the minimum value when its knob is at the bottom.

## See Also

### Asking About the Value Limits

var maxValue: Double

The maximum value the slider can send to its target.

