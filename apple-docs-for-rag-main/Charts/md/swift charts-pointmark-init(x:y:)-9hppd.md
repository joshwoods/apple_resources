

- Swift Charts
- PointMark
-  init(x:y:) 

Initializer

# init(x:y:)

Creates a point mark that plots a value on x with fixed y position.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    y: CGFloat? = nil
) where X : Plottable
```

## Parameters 

`x`  

The value plotted with x.

`y`  

The y position. If `y` is `nil`, the bar will be centered vertically by default.

### Discussion

Use this initializer to plot a property with x:

```
Chart(data) {
    PointMark(
        x: .value("Weight", $0.weight)
    )
}
```

For more background, see the first example used in PointMark which shows the structure that contains the `weight` property.

