

- Swift Charts
- BarMark
-  init(xStart:xEnd:yStart:yEnd:) 

Initializer

# init(xStart:xEnd:yStart:yEnd:)

Creates a bar mark with fixed x interval that plots values with its y interval.

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

## Parameters 

`xStart`  

The x start position. If `xStart` is `nil` then the rectangle will start at the leading edge of the plotting area.

`xEnd`  

The x end position. If `xStart` is `nil` then the rectangle will end at the trailing edge of the plotting area.

`yStart`  

The value plotted to y start.

`yEnd`  

The value plotted to y end.

### Discussion

Use this initializer to show vertical intervals for one category:

```
Chart(data) {
   BarMark(
       yStart: .value("Start Time", $0.start),
       yEnd: .value("End Time", $0.end)
   )
}
```

