

- Accessibility
- AXDataPoint
-  xValue 

Instance Property

# xValue

The value of the x-axis for the data point.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@NSCopying
var xValue: AXDataPointValue { get set }
```

## Discussion

Use a `double` value for a numeric x-axis, or an NSString value for a categorical x-axis.

## See Also

### Specifying the data value

var yValue: AXDataPointValue?

The value of the y-axis for the data point.

class AXDataPointValue

A single data value.

enum Value

Constants that describe types of data values.

