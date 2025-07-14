

- SwiftUI
- View
-  chartYAxis(\_:) 

Instance Method

# chartYAxis(\_:)

Sets the visibility of the y axis.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartYAxis(_ visibility: Visibility) -> some View
```

## See Also

### Axes

func chartXAxis(Visibility) -> some View

Sets the visibility of the x axis.

func chartXAxis&lt;Content>(content: () -> Content) -> some View

Configures the x-axis for charts in the view.

func chartXAxisStyle&lt;Content>(content: (ChartAxisContent) -> Content) -> some View

Configures the x axis content of charts.

func chartYAxis&lt;Content>(content: () -> Content) -> some View

Configures the y-axis for charts in the view.

func chartYAxisStyle&lt;Content>(content: (ChartAxisContent) -> Content) -> some View

Configures the y axis content of charts.

