

- SwiftUI
- View fundamentals
- View
-  Chart view modifiers 

API Collection

# Chart view modifiers

Configure charts that you declare with Swift Charts.

## Overview

Use these modifiers to configure a Chart view that you add to your SwiftUI app.

## Topics

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

func chartPlotStyle&lt;Content>(content: (ChartPlotContent) -> Content) -> some View

Configures the plot area of charts.

### Legends

func chartLegend(Visibility) -> some View

Configures the legend for charts.

func chartLegend(position: AnnotationPosition, alignment: Alignment?, spacing: CGFloat?) -> some View

Configures the legend for charts.

func chartLegend&lt;Content>(position: AnnotationPosition, alignment: Alignment?, spacing: CGFloat?, content: () -> Content) -> some View

Configures the legend for charts.

### Overlays

func chartOverlay&lt;V>(alignment: Alignment, content: (ChartProxy) -> V) -> some View

Adds an overlay to a view that contains a chart.

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

func chartYAxisStyle&lt;Content>(content: (ChartAxisContent) -> Content) -> some View

Configures the y axis content of charts.

### Axis Labels

func chartXAxisLabel(_:position:alignment:spacing:)

Adds x axis label for charts in the view.

func chartXAxisLabel&lt;C>(position: AnnotationPosition, alignment: Alignment?, spacing: CGFloat?, content: () -> C) -> some View

Adds x axis label for charts in the view.

func chartYAxisLabel(_:position:alignment:spacing:)

Adds y axis label for charts in the view.

func chartYAxisLabel&lt;C>(position: AnnotationPosition, alignment: Alignment?, spacing: CGFloat?, content: () -> C) -> some View

Adds y axis label for charts in the view.

### Axis scales

func chartXScale&lt;Domain, Range>(domain: Domain, range: Range, type: ScaleType?) -> some View

Configures the x scale for charts.

func chartXScale&lt;Domain>(domain: Domain, type: ScaleType?) -> some View

Configures the x scale for charts.

func chartXScale&lt;Range>(range: Range, type: ScaleType?) -> some View

Configures the x scale for charts.

func chartXScale(type: ScaleType?) -> some View

Configures the x scale for charts.

func chartYScale&lt;Domain, Range>(domain: Domain, range: Range, type: ScaleType?) -> some View

Configures the y scale for charts.

func chartYScale&lt;Domain>(domain: Domain, type: ScaleType?) -> some View

Configures the y scale for charts.

func chartYScale&lt;Range>(range: Range, type: ScaleType?) -> some View

Configures the y scale for charts.

func chartYScale(type: ScaleType?) -> some View

Configures the y scale for charts.

### Symbol scales

func chartSymbolScale(_:)

Configures the symbol scale for charts.

func chartSymbolScale&lt;Domain>(domain: Domain) -> some View

Configures the symbol style scale for charts.

func chartSymbolScale(domain:range:)

Configures the symbol style scale for charts.

func chartSymbolScale&lt;Domain, S>(domain: Domain, mapping: (Domain.Element) -> S) -> some View

Configures the symbol scale for charts.

func chartSymbolScale&lt;DataValue, S>(mapping: (DataValue) -> S) -> some View

Configures the symbol scale for charts.

func chartSymbolScale(range:)

Configures the symbol style scale for charts.

### Symbol size scales

func chartSymbolSizeScale&lt;DataValue>(KeyValuePairs&lt;DataValue, CGFloat>) -> some View

Configures the symbol size scale for charts.

func chartSymbolSizeScale&lt;Domain, Range>(domain: Domain, range: Range, type: ScaleType?) -> some View

Configures the symbol size scale for charts.

func chartSymbolSizeScale&lt;Domain>(domain: Domain, type: ScaleType?) -> some View

Configures the symbol size scale for charts.

func chartSymbolSizeScale&lt;Domain>(domain: Domain, mapping: (Domain.Element) -> CGFloat) -> some View

Configures the symbol size scale for charts.

func chartSymbolSizeScale&lt;DataValue>(mapping: (DataValue) -> CGFloat) -> some View

Configures the symbol size scale for charts.

func chartSymbolSizeScale&lt;Range>(range: Range, type: ScaleType?) -> some View

Configures the symbol size scale for charts.

func chartSymbolSizeScale(type: ScaleType?) -> some View

Configures the symbol size scale for charts.

### Line style scales

func chartLineStyleScale&lt;DataValue>(KeyValuePairs&lt;DataValue, StrokeStyle>) -> some View

Configures the line style scale for charts.

func chartLineStyleScale&lt;Domain>(domain: Domain) -> some View

Configures the line style scale for charts.

func chartLineStyleScale&lt;Domain, Range>(domain: Domain, range: Range) -> some View

Configures the line style scale for charts.

func chartLineStyleScale&lt;Range>(range: Range) -> some View

Configures the line style scale for charts.

func chartLineStyleScale&lt;Domain>(domain: Domain, mapping: (Domain.Element) -> StrokeStyle) -> some View

Configures the line style scale for charts.

func chartLineStyleScale&lt;DataValue>(mapping: (DataValue) -> StrokeStyle) -> some View

Configures the line style scale for charts.

### Scrolling

func chartScrollPosition(initialX: some Plottable) -> some View

Sets the initial scroll position along the x-axis. Once the user scrolls the scroll view, the value provided to this modifier will have no effect.

func chartScrollPosition(initialY: some Plottable) -> some View

Sets the initial scroll position along the y-axis. Once the user scrolls the scroll view, the value provided to this modifier will have no effect.

func chartScrollPosition(x: Binding&lt;some Plottable>) -> some View

Associates a binding to be updated when the chart scrolls along the x-axis.

func chartScrollPosition(y: Binding&lt;some Plottable>) -> some View

Associates a binding to be updated when the chart scrolls along the y-axis.

func chartScrollTargetBehavior(some ChartScrollTargetBehavior) -> some View

Sets the scroll behavior of the scrollable chart.

func chartScrollableAxes(Axis.Set) -> some View

Configures the scrollable behavior of charts in this view.

### Selection

func chartXSelection&lt;P>(range: Binding&lt;ClosedRange&lt;P>?>) -> some View

func chartXSelection&lt;P>(value: Binding&lt;P?>) -> some View

func chartYSelection&lt;P>(range: Binding&lt;ClosedRange&lt;P>?>) -> some View

func chartYSelection&lt;P>(value: Binding&lt;P?>) -> some View

func chartAngleSelection&lt;P>(value: Binding&lt;P?>) -> some View

### Visible domain

func chartXVisibleDomain&lt;P>(length: P) -> some View

Sets the length of the visible domain in the X dimension.

func chartYVisibleDomain&lt;P>(length: P) -> some View

Sets the length of the visible domain in the Y dimension.

### Interaction

func chartGesture((ChartProxy) -> some Gesture) -> some View

## See Also

### Configuring view elements

Accessibility modifiers

Make your SwiftUI apps accessible to everyone, including people with disabilities.

Appearance modifiers

Configure a view’s foreground and background styles, controls, and visibility.

Text and symbol modifiers

Manage the rendering, selection, and entry of text in your view.

Auxiliary view modifiers

Add and configure supporting views, like toolbars and context menus.

