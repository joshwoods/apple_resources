

- Swift
- Double
-  dataValue 

Instance Property

# dataValue

The value of the conforming type’s instance wrapped in a data value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var dataValue: MLDataValue { get }
```

## See Also

### Using a Double as a Data Value

init?(from: MLDataValue)

Creates an instance of the conforming type from a data value.

static var dataValueType: MLDataValue.ValueType

The underlying type the conforming type uses when it wraps itself in a data value.

