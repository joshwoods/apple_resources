

- Swift Charts
- RectangleMark
-  init(x:yStart:yEnd:width:) 

Initializer

# init(x:yStart:yEnd:width:)

Creates a rectangle mark with an y interval encoding and an x encoding.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    yStart: PlottableValue,
    yEnd: PlottableValue,
    width: MarkDimension = .automatic
) where X : Plottable, Y : Plottable
```

## Parameters 

`x`  

The value plotted with y.

`yStart`  

The value plotted with x start.

`yEnd`  

The value plotted with x end.

`width`  

The rectangle width. If `width` is not specified, then 70% of the step size will be used. If there is no step size a default width (in pts) will be used.

### Discussion

Use this initializer to map the y start, y end and x position to a rectangle for each data element. Optionally, specify the width of the rectangles.

The example below omits the optional `width` field and uses a number scale starting at (0,0) and ending at (6,6). The rectangle has the coordinates: (0,2), (0,4), (4,4), (4,2).

```
Chart(data) {
    RectangleMark(
        yStart: .value("Rect yStart", 2),
        yEnd: .value("Rect yEnd", 4),
        x: .value("Rect X", 4)
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

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, height: MarkDimension)

Creates a rectangle mark with an x interval encoding and a y encoding.

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>)

Creates a rectangle mark with x and y interval encodings.

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, width: MarkDimension, height: MarkDimension)

Creates a rectangle that plots values with x and y.

