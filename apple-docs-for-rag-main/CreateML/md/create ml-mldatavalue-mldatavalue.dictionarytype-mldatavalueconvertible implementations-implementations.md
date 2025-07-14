

- Create ML
- MLDataValue
- MLDataValue.DictionaryType
-  MLDataValueConvertible Implementations 

API Collection

# MLDataValueConvertible Implementations

## Topics

### Initializers

init()

Creates a new default instance of the conforming type when a data value is missing or invalid.

init?(from: MLDataValue)

Creates a data-value dictionary from another dictionary.

### Instance Properties

var dataValue: MLDataValue

The dictionary wrapped in a data value.

### Type Properties

static var dataValueType: MLDataValue.ValueType

The underlying type a machine learning dictionary uses when it wraps itself in a data value.

