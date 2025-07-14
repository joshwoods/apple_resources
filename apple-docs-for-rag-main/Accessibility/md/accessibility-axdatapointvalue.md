

- Accessibility
-  AXDataPointValue 

Class

# AXDataPointValue

A single data value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AXDataPointValue
```

## Overview

An AXDataPointValue can be either numeric or categorical. Data points in a numeric axis use the number property, and data points in a categorical axis use the category property.

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

### Specifying the data value

var xValue: AXDataPointValue

The value of the x-axis for the data point.

var yValue: AXDataPointValue?

The value of the y-axis for the data point.

enum Value

Constants that describe types of data values.

