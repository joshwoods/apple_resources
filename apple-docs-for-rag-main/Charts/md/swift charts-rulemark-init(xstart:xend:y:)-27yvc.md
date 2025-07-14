

- Swift Charts
- RuleMark
-  init(xStart:xEnd:y:) 

Initializer

# init(xStart:xEnd:y:)

Creates a horizontal rule mark that plots values on its x interval and on y.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    xStart: PlottableValue,
    xEnd: PlottableValue,
    y: PlottableValue
) where X : Plottable, Y : Plottable
```

## Parameters 

`xStart`  

The value plotted with x start.

`xEnd`  

The value plotted with x end.

`y`  

The value plotted with y.

### Discussion

Use this initializer to create a horizontal rule at x positions from `xStart` to `xEnd` to a y position:

```
Chart(data) {
    RuleMark(
        xStart: .value("Start Date", $0.startDate),
        xEnd: .value("End Date", $0.endDate),
        y: .value("Pollen Source", $0.source)
    )
}
```

See the second code example in RuleMark for the setup of the structure that contains the `startDate`, `endDate`, and `source` properties.

