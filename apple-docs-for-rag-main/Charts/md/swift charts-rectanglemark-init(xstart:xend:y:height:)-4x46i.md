

- Swift Charts
- RectangleMark
-  init(xStart:xEnd:y:height:) 

Initializer

# init(xStart:xEnd:y:height:)

Creates a rectangle mark with a fixed x interval and y encoding.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    xStart: CGFloat? = nil,
    xEnd: CGFloat? = nil,
    y: PlottableValue,
    height: MarkDimension = .automatic
) where Y : Plottable
```

## Discussion

- xStart: The x start position. If `xStart` is `nil` then the rectangle will start at the leading edge of the plotting area.

- xEnd: The x end position. If `xEnd` is `nil` then the rectangle will end at the trailing edge of the plotting area.

- y: The value plotted with y.

- height: The rectangle height. If `height` is not specified, then 70% of the step size will be used. If there is no step size a default height (in pts) will be used.

### Discussion

Use this initializer to map a y position to a rectangle for each data element. Optionally, specify the height, xStart position, or xEnd position, of the rectangles.

The example below omits the optional `x`, `width`, and `height` parameters and uses a number scale starting at (0,0) and ending at (6,6). The rectangle has the coordinates: (0,0), (0,3), (6,3), (6,0).

```
Chart(data) {
    RectangleMark(
        y: .value("Rect Y", 3)
    )
    .opacity(0.2)

    PointMark(
        x: .value("X", $0.x),
        y: .value("Y", $0.y)
    )
}
```

