

- Swift Charts
- RectangleMark
-  init(xStart:xEnd:yStart:yEnd:) 

Initializer

# init(xStart:xEnd:yStart:yEnd:)

Creates a rectangle mark with x and y interval encodings.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    xStart: PlottableValue,
    xEnd: PlottableValue,
    yStart: PlottableValue,
    yEnd: PlottableValue
) where X : Plottable, Y : Plottable
```

## Parameters 

`xStart`  

The value plotted with x start.

`xEnd`  

The value plotted with x end.

`yStart`  

The value plotted with y start.

`yEnd`  

The value plotted with y end.

### Discussion

Use this initializer to map the x start, x end, y start, and y end position to a rectangle for each data element.

The example below uses a number scale starting at (0,0) and ending at (6,6). The rectangle has the coordinates: (2,2), (2,4), (4,4), (4,2).

```
Chart(data) {
    RectangleMark(
        xStart: .value("Rect xStart", 2),
        xEnd: .value("Rect xEnd", 4),
        yStart: .value("Rect yStart", 2),
        yEnd: .value("Rect yEnd", 4)
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

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, width: MarkDimension, height: MarkDimension)

Creates a rectangle that plots values with x and y.

