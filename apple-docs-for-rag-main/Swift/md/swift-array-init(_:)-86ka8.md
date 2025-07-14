

- Swift
- Array
-  init(\_:) 

Initializer

# init(\_:)

Constructs an Array with the elements of an MLUntypedColumn.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(_ untypedColumn: MLUntypedColumn)
```

Available when `Element` is `MLDataValue`.

## See Also

### Converting Between Arrays and Create ML Types

init(MLDataColumn&lt;Element>)

Constructs an Array with the elements of a DataColumn.

init?(from: MLDataValue)

Creates an instance of the conforming type from a data value.

var dataValue: MLDataValue

The value of the conforming type’s instance wrapped in a data value.

static var dataValueType: MLDataValue.ValueType

The underlying type the conforming type uses when it wraps itself in a data value.

