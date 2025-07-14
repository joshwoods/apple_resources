

- SwiftUI
- View
-  chartForegroundStyleScale(domain:range:type:) 

Instance Method

# chartForegroundStyleScale(domain:range:type:)

Configures the foreground style scale for charts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartForegroundStyleScale(
    domain: Domain,
    range: Range,
    type: ScaleType? = nil
) -> some View where Domain : ScaleDomain, Range : ScaleRange, Range.VisualValue : ShapeStyle
```

## Parameters 

`domain`  

The possible data values plotted as foreground style in the chart. You can define the domain with a `ClosedRange` for number or `Date` values (e.g., `0 ... 500`), and with an array for categorical values (e.g., `["A", "B", "C"]`)

`range`  

The range of foreground styles that correspond to the scale domain.

`type`  

The scale type.

## See Also

### Styles

func chartBackground&lt;V>(alignment: Alignment, content: (ChartProxy) -> V) -> some View

Adds a background to a view that contains a chart.

func chartForegroundStyleScale&lt;DataValue, S>(KeyValuePairs&lt;DataValue, S>) -> some View

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

