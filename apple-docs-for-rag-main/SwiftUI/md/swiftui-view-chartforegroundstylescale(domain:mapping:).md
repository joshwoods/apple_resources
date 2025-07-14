

- SwiftUI
- View
-  chartForegroundStyleScale(domain:mapping:) 

Instance Method

# chartForegroundStyleScale(domain:mapping:)

Configures the foreground style scale for charts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartForegroundStyleScale(
    domain: Domain,
    mapping: @escaping (Domain.Element) -> S
) -> some View where Domain : Collection, S : ShapeStyle, Domain.Element : Plottable
```

## Parameters 

`domain`  

The possible data values plotted as foreground style in the chart.

`mapping`  

Maps data categories to foreground styles.

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

func chartForegroundStyleScale&lt;DataValue, S>(mapping: (DataValue) -> S) -> some View

Configures the foreground style scale for charts.

func chartForegroundStyleScale&lt;Range>(range: Range, type: ScaleType?) -> some View

Configures the foreground style scale for charts.

func chartForegroundStyleScale(type: ScaleType?) -> some View

Configures the foreground style scale for charts.

func chartPlotStyle&lt;Content>(content: (ChartPlotContent) -> Content) -> some View

Configures the plot area of charts.

