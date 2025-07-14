

- Swift Charts
- RuleMark
-  init(xStart:xEnd:y:) 

Initializer

# init(xStart:xEnd:y:)

Creates a horizontal rule mark that plots a value on y.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    xStart: CGFloat? = nil,
    xEnd: CGFloat? = nil,
    y: PlottableValue
) where Y : Plottable
```

## Parameters 

`xStart`  

The x start position. If `xStart` is `nil` the rule will start at the leading edge of the plotting area.

`xEnd`  

The x end position. If `xEnd` is `nil` the rule will end at the trailing edge of the plotting area.

`y`  

The value plotted with y.

### Discussion

Use this initializer to create a horizontal rule across a chart’s plotting area at a y position:

```
Chart {
    ForEach(data) {
        BarMark(
            x: .value("Department", $0.department),
            y: .value("Profit", $0.profit)
        )
    }
    RuleMark(y: .value("Break Even Threshold", 9000))
        .foregroundStyle(.red)
}
```

See the first code example in RuleMark for the setup of the structure that contains the `department` and `profit` properties.

