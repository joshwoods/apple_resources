

- SwiftUI
- View
-  chartYAxisStyle(content:) 

Instance Method

# chartYAxisStyle(content:)

Configures the y axis content of charts.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func chartYAxisStyle(@ViewBuilder content: @escaping (ChartAxisContent) -> Content) -> some View where Content : View
```

## Parameters 

`content`  

A closure that returns the content of the axis.

## Discussion

Use this modifier to configure the size or aspect ratio of the plot area of charts.

For example:

```
Chart(data: data) {
    BarMark(x: .value("Category", $0.category))
}
.chartYAxisStyle { axis in
    axis.opacity(0.5)
}
```

## See Also

### Axes

func chartXAxis(Visibility) -> some View

Sets the visibility of the x axis.

func chartXAxis&lt;Content>(content: () -> Content) -> some View

Configures the x-axis for charts in the view.

func chartXAxisStyle&lt;Content>(content: (ChartAxisContent) -> Content) -> some View

Configures the x axis content of charts.

func chartYAxis(Visibility) -> some View

Sets the visibility of the y axis.

func chartYAxis&lt;Content>(content: () -> Content) -> some View

Configures the y-axis for charts in the view.

