

- SwiftUI
- View
-  chartBackground(alignment:content:) 

Instance Method

# chartBackground(alignment:content:)

Adds a background to a view that contains a chart.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartBackground(
    alignment: Alignment = .center,
    @ViewBuilder content: @escaping (ChartProxy) -> V
) -> some View where V : View
```

## Parameters 

`alignment`  

The alignment of the content.

`content`  

The content of the background.

## Discussion

You can use this modifier to define a background view as a function of the chart in the view. You can access the chart with the `ChartProxy` object passed into the closure.

Note

If `self` contains more than one chart, the chart proxy will refer to the first chart.

## See Also

### Styles

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

func chartPlotStyle&lt;Content>(content: (ChartPlotContent) -> Content) -> some View

Configures the plot area of charts.

