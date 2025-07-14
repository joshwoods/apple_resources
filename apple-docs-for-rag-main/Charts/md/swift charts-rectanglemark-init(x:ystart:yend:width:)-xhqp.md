

- Swift Charts
- RectangleMark
-  init(x:yStart:yEnd:width:) 

Initializer

# init(x:yStart:yEnd:width:)

Creates a rectangle mark that plots values on x and has a fixed y interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    yStart: CGFloat? = nil,
    yEnd: CGFloat? = nil,
    width: MarkDimension = .automatic
) where X : Plottable
```

## Discussion

- x: The value plotted with x.

- width: The rectangle width. If `width` is not specified, then 70% of the step size will be used. If there is no step size a default width (in pts) will be used.

- yStart: The y start position. If `yStart` is `nil` then the rectangle will start at the leading edge of the plotting area.

- yEnd: The y end position. If `yEnd` is `nil` then the rectangle will end at the trailing edge of the plotting area.

### Discussion

Use this initializer to map an x position to a rectangle for each data element. Optionally, specify the width, yStart position, or yEnd positions of the rectangles.

The example below omits the optional `width`, `yStart`, and `yEnd` parameters and uses a number scale starting at (0,0) and ending at (6,6). The rectangle has the coordinates: (0,0), (0,6), (3,6), (3,0).

```
Chart(data) {
    RectangleMark(
        x: .value("Rect X", 3)
    )
    .opacity(0.2)

    PointMark(
        x: .value("X", $0.x),
        y: .value("Y", $0.y)
    )
}
```

