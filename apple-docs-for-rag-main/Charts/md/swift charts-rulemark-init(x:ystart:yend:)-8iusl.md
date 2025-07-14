

- Swift Charts
- RuleMark
-  init(x:yStart:yEnd:) 

Initializer

# init(x:yStart:yEnd:)

Creates a vertical rule mark with a fixed x position and y interval encoding.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: CGFloat? = nil,
    yStart: PlottableValue,
    yEnd: PlottableValue
) where Y : Plottable
```

## Parameters 

`x`  

The x position. If `x` is `nil`, the rule will be centered horizontally by default.

`yStart`  

The value plotted with y start.

`yEnd`  

The value plotted with y end.

### Discussion

Use this initializer to create a vertical rule at y positions from `yStart` to `yEnd` for a single x position:

```
Chart(data) {
    RuleMark(
        yStart: .value("Start Date", $0.startDate),
        yEnd: .value("End Date", $0.endDate)
    )
}
```

See RuleMark for the setup of the structure containing the `startDate`, `endDate`, and `source` properties.

