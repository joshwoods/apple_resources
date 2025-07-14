

- Swift Charts
- RectangleMark
-  init(x:y:width:height:) 

Initializer

# init(x:y:width:height:)

Creates a rectangle that plots values with x and y.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    y: PlottableValue,
    width: MarkDimension = .automatic,
    height: MarkDimension = .automatic
) where X : Plottable, Y : Plottable
```

## Parameters 

`x`  

The value plotted with x.

`y`  

The value plotted with y.

`width`  

The rectangle width. If `width` is not specified, then 70% of the step size will be used. If there is no step size a default width (in pts) will be used.

`height`  

The rectangle height. If `height` is not specified, then 70% of the step size will be used. If there is no step size a default height (in pts) will be used.

### Discussion

Use this initializer to map an x and y position to a rectangle for each data element. Optionally, specify the width or height of the rectangles.

The example below omits the optional `width` and `height` parameters and uses a number scale starting at (0,0). The rectangle has the coordinates: (0,0), (0,3), (3,0), (3,3).

```
Chart(data) {
    RectangleMark(
        x: .value("Rect X", 3),
        y: .value("Rect Y", 3)
    )
    .opacity(0.2)

    PointMark(
        x: .value("X", $0.x),
        y: .value("Y", $0.y)
    )
}
```

## See Also

### Creating a rectangle mark

init&lt;X, Y>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>, width: MarkDimension)

Creates a rectangle mark with an y interval encoding and an x encoding.

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, height: MarkDimension)

Creates a rectangle mark with an x interval encoding and a y encoding.

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>)

Creates a rectangle mark with x and y interval encodings.

