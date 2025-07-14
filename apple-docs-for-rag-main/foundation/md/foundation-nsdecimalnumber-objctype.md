

- Foundation
- NSDecimalNumber
-  objCType 

Instance Property

# objCType

A C string containing the Objective-C type for the data contained in the decimal number object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var objCType: UnsafePointer { get }
```

## Discussion

For a decimal number object, this property always contains “d” (for double).

## See Also

### Accessing the Value

var decimalValue: Decimal

The decimal number’s value, expressed as an Decimal structure.

var doubleValue: Double

The decimal number’s closest approximate `double` value.

func description(withLocale: Any?) -> String

