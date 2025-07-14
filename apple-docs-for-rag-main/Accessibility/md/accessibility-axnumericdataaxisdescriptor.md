

- Accessibility
-  AXNumericDataAxisDescriptor 

Class

# AXNumericDataAxisDescriptor

An object that represents an axis of numerical data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AXNumericDataAxisDescriptor
```

## Topics

### Creating a numeric data axis

convenience init(title: String, range: ClosedRange&lt;Double>, gridlinePositions: [Double], valueDescriptionProvider: (Double) -> String)

Creates a numeric data axis with the specified title, range, gridline positions, and value description provider closure.

convenience init(attributedTitle: NSAttributedString, range: ClosedRange&lt;Double>, gridlinePositions: [Double], valueDescriptionProvider: (Double) -> String)

Creates a numeric data axis with the specified attributed title, range, gridline positions, and value description provider closure.

### Specifying the value description

var valueDescriptionProvider: (Double) -> String

A description to speak for a particular data value on the axis.

### Configuring the axis scale

var scaleType: AXNumericDataAxisDescriptor.ScaleType

The scale for the axis.

enum ScaleType

Constants that describe the scale of a numeric axis.

### Configuring the axis range

var range: ClosedRange&lt;Double>

A range that defines the minimum and maximum displayable values for the axis.

### Configuring the gridlines

var gridlinePositions: [Double]

The positions of the gridlines along the axis.

## Relationships

### Inherits From

- NSObject

### Conforms To

- AXDataAxisDescriptor
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Axis representation

protocol AXDataAxisDescriptor

The basic interface for a data axis in a chart.

class AXCategoricalDataAxisDescriptor

An object that represents an axis of categorical data.

