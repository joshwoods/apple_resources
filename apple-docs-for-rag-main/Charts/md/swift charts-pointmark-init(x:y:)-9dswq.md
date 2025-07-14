

- Swift Charts
- PointMark
-  init(x:y:) 

Initializer

# init(x:y:)

Creates a point mark with fixed x position and plots values with y.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: CGFloat? = nil,
    y: PlottableValue
) where Y : Plottable
```

## Parameters 

`x`  

The x position. If `x` is `nil`, the bar will be centered horizontally by default.

`y`  

The value plotted with y.

### Discussion

Use this initializer to plot a property to y:

```
Chart(data) {
    PointMark(
        y: .value("Weight", $0.weight)
    )
}
```

For more background, see the first example used in PointMark which shows the structure that contains the `weight` property.

