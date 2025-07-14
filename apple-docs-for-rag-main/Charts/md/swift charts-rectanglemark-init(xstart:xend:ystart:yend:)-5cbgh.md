

- Swift Charts
- RectangleMark
-  init(xStart:xEnd:yStart:yEnd:) 

Initializer

# init(xStart:xEnd:yStart:yEnd:)

Creates a rectangle mark with a y interval encoding and a fixed x interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    xStart: CGFloat? = nil,
    xEnd: CGFloat? = nil,
    yStart: PlottableValue,
    yEnd: PlottableValue
) where Y : Plottable
```

## Discussion

- yStart: The value plotted with y end.

- yEnd: The value plotted with y end.

- xStart: The x start position. If `xStart` is `nil` then the rectangle will start at the leading edge of the plotting area.

- xEnd: The x end position. If `xEnd` is `nil` then the rectangle will end at the trailing edge of the plotting area.

### Discussion

Use this initializer to map the y start and y end position to a rectangle for each data element. Optionally, specify the xStart or xEnd position of the rectangles.

The example below omits the optional `x` and `width` fields and uses a number scale starting at (0,0) and ending at (6,6). The rectangle has the coordinates: (0,2), (0,4), (6,4), (6,2).

```
Chart(data) {
    RectangleMark(
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

