

- Accessibility
-  AXDataSeriesDescriptor 

Class

# AXDataSeriesDescriptor

An object that represents a series of data points.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AXDataSeriesDescriptor
```

## Topics

### Creating a data series

init(name: String, isContinuous: Bool, dataPoints: [AXDataPoint])

Creates a data series with the specified name, a Boolean value that indicates whether the series is continuous, and data points.

init(attributedName: NSAttributedString, isContinuous: Bool, dataPoints: [AXDataPoint])

Creates a data series with the specified attributed name, a Boolean value that indicates whether the series is continuous, and data points.

### Naming the series

var name: String?

The name of the data series.

var attributedName: NSAttributedString

An attributed version of the data series name.

### Configuring the data points

var isContinuous: Bool

A Boolean value that determines whether the data series is continuous.

var dataPoints: [AXDataPoint]

The data points that the series contains.

class AXDataPoint

An object that represents a single data point in a chart.

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

class AXDataPoint

An object that represents a single data point in a chart.

