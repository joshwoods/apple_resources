

- Create ML
- MLDataValue
- MLDataValue.SequenceType
-  MLDataValueConvertible Implementations 

API Collection

# MLDataValueConvertible Implementations

## Topics

### Initializers

init()

Creates a new default instance of the conforming type when a data value is missing or invalid.

init?(from: MLDataValue)

Creates a data-value sequence from another sequence.

### Instance Properties

var dataValue: MLDataValue

The sequence wrapped in a data value.

### Type Properties

static var dataValueType: MLDataValue.ValueType

The underlying type a machine learning sequence uses when it wraps itself in a data value.

