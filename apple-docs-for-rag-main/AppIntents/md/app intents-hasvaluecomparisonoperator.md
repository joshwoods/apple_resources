

- App Intents
-  HasValueComparisonOperator 

Enumeration

# HasValueComparisonOperator

Operators that indicate the type of value check for a conditional statement.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum HasValueComparisonOperator
```

## Topics

### Value operators

case hasAnyValue

An operator that determines if the parameter has a value.

case hasNoValue

An operator that determines if the parameter’s empty.

### Operators

static func == (HasValueComparisonOperator, HasValueComparisonOperator) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Creating a conditional statement

init&lt;Parameter>(KeyPath&lt;Intent, Parameter>, HasValueComparisonOperator, () -> WhenCondition, otherwise: () -> Otherwise)

enum EquatableComparisonOperator

Operators that indicate the type of equality check for a conditional statement.

enum ComparableComparisonOperator

Operators that indicate the type of comparison check for a conditional statement.

enum OneOfComparisonOperator

Operators that indicate the type of containment check for a conditional statement.

