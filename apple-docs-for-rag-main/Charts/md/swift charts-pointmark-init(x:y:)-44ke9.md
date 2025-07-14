

- Swift Charts
- PointMark
-  init(x:y:) 

Initializer

# init(x:y:)

Creates a point mark that plots values to x and y.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    y: PlottableValue
) where X : Plottable, Y : Plottable
```

## Parameters 

`x`  

The value plotted with x.

`y`  

The value plotted with y.

### Discussion

Use this initializer to plot one property with x and another property with y:

```
Chart(data) {
    PointMark(
        x: .value("Wing Length", $0.wingLength),
        y: .value("Wing Length", $0.wingWidth)
    )
}
```

For more background, see the first example used in PointMark which shows the structure that contains the `wingLength` and `wingHeight` properties.

