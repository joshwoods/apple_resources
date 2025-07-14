

- Foundation
- NSDecimalNumber
-  doubleValue 

Instance Property

# doubleValue

The decimal number’s closest approximate `double` value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var doubleValue: Double { get }
```

## Discussion

Not all decimal numbers can be accurately represented using a `double` value.

## See Also

### Accessing the Value

var decimalValue: Decimal

The decimal number’s value, expressed as an Decimal structure.

func description(withLocale: Any?) -> String

var objCType: UnsafePointer&lt;CChar>

A C string containing the Objective-C type for the data contained in the decimal number object.

