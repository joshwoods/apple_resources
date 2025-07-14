

- AppKit
- NSSlider
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

The slider’s maximum value. A horizontal slider sends the maximum value when the knob is all the way to the trailing end of the bar. A vertical slider sends the maximum value when the knob is at the top.

## See Also

### Asking About the Value Limits

var minValue: Double

The minimum value the slider can send to its target.

