

- Swift
- Dictionary
-  dataValue 

Instance Property

# dataValue

The value of the conforming type’s instance wrapped in a data value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var dataValue: MLDataValue { get }
```

Available when `Key` conforms to `MLDataValueConvertible`, `Key` conforms to `Hashable`, and `Value` conforms to `MLDataValueConvertible`.

## See Also

### Converting Between Dictionaries and Create ML Types

init?(from: MLDataValue)

Creates an instance of the conforming type from a data value.

static var dataValueType: MLDataValue.ValueType

The underlying type the conforming type uses when it wraps itself in a data value.

