

- AppKit
- NSLevelIndicatorCell
-  numberOfMajorTickMarks 

Instance Property

# numberOfMajorTickMarks

The number of major tick marks displayed by the control.

macOS

``` source
@MainActor
var numberOfMajorTickMarks: Int { get set }
```

## Discussion

The value in this property must be less than or equal to the value in the numberOfTickMarks property.

## See Also

### Managing Tick Marks

var tickMarkPosition: NSSlider.TickMarkPosition

The placement of tick marks on the level indicator control.

var numberOfTickMarks: Int

The number of tick marks displayed by the control.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at index (the minimum-value tick mark has an index of 0).

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark identified by `index` (the minimum-value tick mark is at index 0).

