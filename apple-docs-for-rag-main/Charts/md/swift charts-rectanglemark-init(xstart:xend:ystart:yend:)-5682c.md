

- Swift Charts
- RectangleMark
-  init(xStart:xEnd:yStart:yEnd:) 

Initializer

# init(xStart:xEnd:yStart:yEnd:)

Creates a rectangle mark with fixed x and y intervals.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    xStart: CGFloat? = nil,
    xEnd: CGFloat? = nil,
    yStart: CGFloat? = nil,
    yEnd: CGFloat? = nil
)
```

## Discussion

- xStart: The x start position. If `xStart` is `nil` then the rectangle will start at the leading edge of the plotting area.

- xEnd: The x end position. If `xEnd` is `nil` then the rectangle will end at the trailing edge of the plotting area.

- yStart: The y start position. If `yStart` is `nil` then the rectangle will start at the leading edge of the plotting area.

- yEnd: The y end position. If `yEnd` is `nil` then the rectangle will end at the trailing edge of the plotting area.

### Discussion

Use this initializer to create one rectangle with any optional x start, x end, y start, and y end position. If no parameters are specified the rectangle will fill the plotting area of the chart.

The example below uses a number scale starting at (0,0) and ending at (6,6). The rectangle has the coordinates: (2,2), (2,4), (4,4), (4,2).

```
Chart(data) {
    RectangleMark()
        .opacity(0.2)

    PointMark(
        x: .value("X", $0.x),
        y: .value("Y", $0.y)
    )
}
```

