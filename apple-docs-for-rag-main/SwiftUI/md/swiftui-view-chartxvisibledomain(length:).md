

- SwiftUI
- View
-  chartXVisibleDomain(length:) 

Instance Method

# chartXVisibleDomain(length:)

Sets the length of the visible domain in the X dimension.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func chartXVisibleDomain(length: P) -> some View where P : Plottable, P : Numeric
```

## Parameters 

`length`  

The length of the visible domain measured in data units. For categorical data, this should be the number of visible categories.

## Discussion

Use this method to control how much of the chart is visible in a scrollable chart. The example below sets the visible portion of the chart to 10 units in the X axis.

```
Chart(data) {
    BarMark(
        x: .value("x", $0.x),
        y: .value("y", $0.y)
    )
}
.chartScrollableAxes(.horizontal)
.chartXVisibleDomain(length: 10)
```

## See Also

### Visible domain

func chartYVisibleDomain&lt;P>(length: P) -> some View

Sets the length of the visible domain in the Y dimension.

