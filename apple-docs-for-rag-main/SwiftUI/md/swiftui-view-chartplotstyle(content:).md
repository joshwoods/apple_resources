

- SwiftUI
- View
-  chartPlotStyle(content:) 

Instance Method

# chartPlotStyle(content:)

Configures the plot area of charts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartPlotStyle(@ViewBuilder content: @escaping (ChartPlotContent) -> Content) -> some View where Content : View
```

## Parameters 

`content`  

A closure that returns the content of the plot area.

## Discussion

Use this modifier to configure the size or aspect ratio of the plot area of charts.

For example:

```
Chart(data: data) {
    BarMark(x: .value("Category", $0.category))
}
.chartPlotStyle { content in
    content.frame(width: 100, height: 100)
}
```

## See Also

### Styles

func chartBackground&lt;V>(alignment: Alignment, content: (ChartProxy) -> V) -> some View

Adds a background to a view that contains a chart.

func chartForegroundStyleScale&lt;DataValue, S>(KeyValuePairs&lt;DataValue, S>) -> some View

Configures the foreground style scale for charts.

func chartForegroundStyleScale&lt;Domain, Range>(domain: Domain, range: Range, type: ScaleType?) -> some View

Configures the foreground style scale for charts.

func chartForegroundStyleScale&lt;Domain>(domain: Domain, type: ScaleType?) -> some View

Configures the foreground style scale for charts.

func chartForegroundStyleScale&lt;Domain, S>(domain: Domain, mapping: (Domain.Element) -> S) -> some View

Configures the foreground style scale for charts.

func chartForegroundStyleScale&lt;DataValue, S>(mapping: (DataValue) -> S) -> some View

Configures the foreground style scale for charts.

func chartForegroundStyleScale&lt;Range>(range: Range, type: ScaleType?) -> some View

Configures the foreground style scale for charts.

func chartForegroundStyleScale(type: ScaleType?) -> some View

Configures the foreground style scale for charts.

