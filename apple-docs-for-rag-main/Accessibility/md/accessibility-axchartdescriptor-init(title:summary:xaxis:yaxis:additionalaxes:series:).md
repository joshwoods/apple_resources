

- Accessibility
- AXChartDescriptor
-  init(title:summary:xAxis:yAxis:additionalAxes:series:) 

Initializer

# init(title:summary:xAxis:yAxis:additionalAxes:series:)

Creates a chart descriptor with the specified title, summary, x-axis descriptor, y-axis descriptor, descriptors for additional axes, and array of data series.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
convenience init(
    title: String? = nil,
    summary: String? = nil,
    xAxis: any AXDataAxisDescriptor,
    yAxis: AXNumericDataAxisDescriptor? = nil,
    additionalAxes: [any AXDataAxisDescriptor] = [],
    series: [AXDataSeriesDescriptor]
)
```

## See Also

### Creating a chart

convenience init(attributedTitle: NSAttributedString?, summary: String?, xAxis: any AXDataAxisDescriptor, yAxis: AXNumericDataAxisDescriptor?, additionalAxes: [any AXDataAxisDescriptor], series: [AXDataSeriesDescriptor])

Creates a chart descriptor with the specified attributed title, summary, x-axis descriptor, y-axis descriptor, descriptors for additional axes, and array of data series.

