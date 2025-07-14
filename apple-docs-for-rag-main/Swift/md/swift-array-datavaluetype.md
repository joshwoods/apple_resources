

- Swift
- Array
-  dataValueType 

Type Property

# dataValueType

The underlying type the conforming type uses when it wraps itself in a data value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static var dataValueType: MLDataValue.ValueType { get }
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Discussion

See `MLDataValue/ValueType` for a list of available options.

## See Also

### Converting Between Arrays and Create ML Types

init(MLDataColumn&lt;Element>)

Constructs an Array with the elements of a DataColumn.

init(MLUntypedColumn)

Constructs an Array with the elements of an MLUntypedColumn.

init?(from: MLDataValue)

Creates an instance of the conforming type from a data value.

var dataValue: MLDataValue

The value of the conforming type’s instance wrapped in a data value.

