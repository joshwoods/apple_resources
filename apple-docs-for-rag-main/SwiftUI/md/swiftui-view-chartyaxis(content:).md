

- SwiftUI
- View
-  chartYAxis(content:) 

Instance Method

# chartYAxis(content:)

Configures the y-axis for charts in the view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartYAxis(@AxisContentBuilder content: () -> Content) -> some View where Content : AxisContent
```

## Parameters 

`content`  

The axis content.

## Discussion

Use this modifier to customize the y-axis of a chart. Provide an `AxisMarks` builder that composes `AxisGridLine`, `AxisTick`, and `AxisValueLabel` structures to form the axis. Omit components from the builder to omit them from the resulting axis. For example, the following code adds grid lines to the y-axis:

```
.chartYAxis {
    AxisMarks {
        AxisGridLine()
    }
}
```

Use arguments such as `position:` or `values:` to control the placement of the axis values it displays.

```
Chart(BatteryData.data, id: \.date) {
     BarMark(
         x: .value("Time", $0.date ..

The above code customizes the y-axis to appear on the leading edge of the chart, with a solid grid line at the 0% and 100% marks.

Note

To add an axis label, use one of the label modifiers, like chartYAxisLabel(position:alignment:spacing:content:).

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

func chartYAxisStyle&lt;Content>(content: (ChartAxisContent) -> Content) -> some View

Configures the y axis content of charts.

