

- Create ML
- MLDataValue
- MLDataValue.MultiArrayType
-  MLDataValueConvertible Implementations 

API Collection

# MLDataValueConvertible Implementations

## Topics

### Initializers

init()

Creates a new default instance of the conforming type when a data value is missing or invalid.

init?(from: MLDataValue)

Creates a data-value multidimensional array from another instance.

### Instance Properties

var dataValue: MLDataValue

The multidimensional array wrapped in a data value.

### Type Properties

static var dataValueType: MLDataValue.ValueType

The underlying type a machine learning multidimensional array uses when it wraps itself in a data value.

