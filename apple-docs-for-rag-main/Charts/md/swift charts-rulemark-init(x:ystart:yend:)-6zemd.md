

- Swift Charts
- RuleMark
-  init(x:yStart:yEnd:) 

Initializer

# init(x:yStart:yEnd:)

Creates a vertical rule mark with value plotted with x.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    yStart: CGFloat? = nil,
    yEnd: CGFloat? = nil
) where X : Plottable
```

## Parameters 

`x`  

The value plotted with x.

`yStart`  

The y start position. If `yStart` is `nil` the rule will start at the leading edge of the plotting area.

`yEnd`  

The y end position. If `yEnd` is `nil` the rule will end at the trailing edge of the plotting area.

### Discussion

Use this initializer to create a vertical rule across a chart’s plotting area at an x position:

```
Chart {
    ForEach(data) {
        BarMark(
            x: .value("Profit", $0.profit),
            y: .value("Department", $0.department)
        )
    }
    RuleMark(x: .value("Break Even Threshold", 9000))
        .foregroundStyle(.red)
}
```

See the first code example in RuleMark for the setup of the structure that contains `department` and `profit` properties.

