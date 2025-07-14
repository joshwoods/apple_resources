

- Swift Charts
- BarMark
-  init(xStart:xEnd:yStart:yEnd:) 

Initializer

# init(xStart:xEnd:yStart:yEnd:)

Creates a bar mark that plots values with its x interval and fixed y position.

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

## Parameters 

`xStart`  

The value plotted with x start.

`xEnd`  

The value plotted with x end.

### Discussion

Use this initializer to show horizontal intervals for one category:

```
Chart(data) {
   BarMark(
       xStart: .value("Start Time", $0.start),
       xEnd: .value("End Time", $0.end)
   )
}
```

