

- Swift Charts
- RectangleMark
-  init(xStart:xEnd:yStart:yEnd:) 

Initializer

# init(xStart:xEnd:yStart:yEnd:)

Creates a rectangle mark with an x interval encoding and a fixed y interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    xStart: PlottableValue,
    xEnd: PlottableValue,
    yStart: CGFloat? = nil,
    yEnd: CGFloat? = nil
) where X : Plottable
```

## Discussion

- xStart: The value plotted with x start.

- xEnd: The value plotted with x end.

- yStart: The y end position. If `yStart` is `nil` then the rectangle will start at the leading edge of the plotting area.

- yEnd: The y end position. If `yEnd` is `nil` then the rectangle will end at the trailing edge of the plotting area.

### Discussion

Use this initializer to map the x start and x end to a rectangle for each data element. Optionally, specify the yStart or yEnd position of the rectangles.

The example below omits the optional `y` and `height` fields and uses a number scale starting at (0,0) and ending at (6,6). The rectangle has the coordinates: (2,0), (2,6), (4,6), (4,0).

```
Chart(data) {
    RectangleMark(
        xStart: .value("Rect xStart", 2),
        xEnd: .value("Rect xEnd", 4)
    )
    .opacity(0.2)

    PointMark(
        x: .value("X", $0.x),
        y: .value("Y", $0.y)
    )
}
```

