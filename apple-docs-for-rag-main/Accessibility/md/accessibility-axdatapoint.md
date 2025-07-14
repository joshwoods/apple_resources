

- Accessibility
-  AXDataPoint 

Class

# AXDataPoint

An object that represents a single data point in a chart.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AXDataPoint
```

## Topics

### Creating a data point

convenience init(x: String, y: Double?, additionalValues: [AXDataPoint.Value], label: String?)

Creates a data point with the specified x-value, y-value, additional values, and label.

convenience init(x: Double, y: Double?, additionalValues: [AXDataPoint.Value], label: String?)

Creates a data point with the specified x-value, y-value, additional values, and label.

### Specifying the data value

var xValue: AXDataPointValue

The value of the x-axis for the data point.

var yValue: AXDataPointValue?

The value of the y-axis for the data point.

class AXDataPointValue

A single data value.

enum Value

Constants that describe types of data values.

### Specifying the label

var label: String?

The label for the data point.

var attributedLabel: NSAttributedString?

An attributed version of the label for the data point.

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

### Data representation

class AXDataSeriesDescriptor

An object that represents a series of data points.

