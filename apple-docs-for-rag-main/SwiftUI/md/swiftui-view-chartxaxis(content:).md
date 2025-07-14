

- SwiftUI
- View
-  chartXAxis(content:) 

Instance Method

# chartXAxis(content:)

Configures the x-axis for charts in the view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartXAxis(@AxisContentBuilder content: () -> Content) -> some View where Content : AxisContent
```

## Parameters 

`content`  

The axis content.

## Discussion

Use this modifier to customize the x-axis of a chart. Provide an `AxisMarks` builder that composes `AxisGridLine`, `AxisTick`, and `AxisValueLabel` structures to form the axis. Omit components from the builder to omit them from the resulting axis. For example, the following code adds grid lines to the x-axis:

```
.chartXAxis {
    AxisMarks {
        AxisGridLine()
    }
}
```

You can also compose multiple `AxisMarks` to create more complex axes:

```
Chart(BatteryData.data, id: \.date) {
     BarMark(
         x: .value("Time", $0.date ..

The above example above customizes the x-axis using two `AxisMarks` declarations. The first creates a grid line for every hour in the day. The second adds a tick and label for every six hours in the day, with a second line showing the date for the very beginning of the axis.

Note

To add an axis label, use one of the label modifiers, like chartXAxisLabel(position:alignment:spacing:content:).

## See Also

### Axes

func chartXAxis(Visibility) -> some View

Sets the visibility of the x axis.

func chartXAxisStyle&lt;Content>(content: (ChartAxisContent) -> Content) -> some View

Configures the x axis content of charts.

func chartYAxis(Visibility) -> some View

Sets the visibility of the y axis.

func chartYAxis&lt;Content>(content: () -> Content) -> some View

Configures the y-axis for charts in the view.

func chartYAxisStyle&lt;Content>(content: (ChartAxisContent) -> Content) -> some View

Configures the y axis content of charts.

