

- Accessibility
-  AXChartDescriptor 

Class

# AXChartDescriptor

An object that contains all the semantic information about an accessible chart.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AXChartDescriptor
```

## Mentioned in 

Representing chart data as an audio graph

## Topics

### Creating a chart

convenience init(title: String?, summary: String?, xAxis: any AXDataAxisDescriptor, yAxis: AXNumericDataAxisDescriptor?, additionalAxes: [any AXDataAxisDescriptor], series: [AXDataSeriesDescriptor])

Creates a chart descriptor with the specified title, summary, x-axis descriptor, y-axis descriptor, descriptors for additional axes, and array of data series.

convenience init(attributedTitle: NSAttributedString?, summary: String?, xAxis: any AXDataAxisDescriptor, yAxis: AXNumericDataAxisDescriptor?, additionalAxes: [any AXDataAxisDescriptor], series: [AXDataSeriesDescriptor])

Creates a chart descriptor with the specified attributed title, summary, x-axis descriptor, y-axis descriptor, descriptors for additional axes, and array of data series.

### Specifying the chart title

var title: String?

The title of the chart.

var attributedTitle: NSAttributedString?

An attributed version of the chart title.

### Specifying the chart summary

var summary: String?

A description of the key takeaways or features of the chart.

### Specifying the axes

var xAxis: any AXDataAxisDescriptor

The axis descriptor for the chart’s x-axis.

var yAxis: AXNumericDataAxisDescriptor?

The axis descriptor for the chart’s y-axis.

var additionalAxes: [any AXDataAxisDescriptor]

The descriptors for additional categorical or numerical axes beyond the x-axis and y-axis.

protocol AXDataAxisDescriptor

The basic interface for a data axis in a chart.

### Specifying a series of data points

var series: [AXDataSeriesDescriptor]

The descriptors for each data series in the chart.

class AXDataSeriesDescriptor

An object that represents a series of data points.

### Specifying the content layout

var contentFrame: CGRect

The bounds of the view, in screen coordinates, for visually rendering data values.

var contentDirection: AXChartDescriptor.ContentDirection

The direction of the content in the chart.

enum ContentDirection

A constant that describes the content direction of the chart.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Chart representation

protocol AXChart

A protocol that declares the minimum interface necessary for an accessibility element to act as a chart.

