

- Swift Charts
- RuleMark
-  init(x:yStart:yEnd:) 

Initializer

# init(x:yStart:yEnd:)

Creates a vertical rule mark with an x encoding and y interval encoding.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    yStart: PlottableValue,
    yEnd: PlottableValue
) where X : Plottable, Y : Plottable
```

## Parameters 

`x`  

The value plotted with x.

`yStart`  

The value plotted with y start.

`yEnd`  

The value plotted with y end.

### Discussion

Use this initializer to create a vertical line at y positions from `yStart` to `yEnd` to an x position:

```
Chart(data) {
    RuleMark(
        x: .value("Pollen Source", $0.source),
        yStart: .value("Start Date", $0.startDate),
        yEnd: .value("End Date", $0.endDate)
    )
}
```

See RuleMark for the setup of the structure that contains the `startDate`, `endDate`, and `source` properties.

