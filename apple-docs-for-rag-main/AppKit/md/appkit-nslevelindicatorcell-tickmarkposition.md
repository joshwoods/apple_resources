

- AppKit
- NSLevelIndicatorCell
-  tickMarkPosition 

Instance Property

# tickMarkPosition

The placement of tick marks on the level indicator control.

macOS

``` source
@MainActor
var tickMarkPosition: NSSlider.TickMarkPosition { get set }
```

## Discussion

Use this property to set the position where the control draws tick marks. Regardless of the value in this property, tick marks are not drawn if the value in the numberOfTickMarks property is `0`.

The default value of this property is NSTickMarkBelow, which also corresponds to the value NSTickMarkLeft for vertically oriented level indicators.

## See Also

### Managing Tick Marks

var numberOfTickMarks: Int

The number of tick marks displayed by the control.

var numberOfMajorTickMarks: Int

The number of major tick marks displayed by the control.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at index (the minimum-value tick mark has an index of 0).

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark identified by `index` (the minimum-value tick mark is at index 0).

