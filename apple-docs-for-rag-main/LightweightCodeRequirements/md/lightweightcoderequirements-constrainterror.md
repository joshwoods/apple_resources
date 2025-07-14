

- LightweightCodeRequirements
-  ConstraintError 

Enumeration

# ConstraintError

Error types that can be thrown from lightweight code requirement routines.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
enum ConstraintError
```

## Topics

### Operators

static func == (ConstraintError, ConstraintError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case duplicateKey

Two constraints of the same type were found in the same logical group.

case malformedConstraint

An unexpected type was found when trying to encode or decode a constraint.

case taskIsNoLongerValid

A SecTask operation failed because the task is no longer valid

case unsupportedConstraintForRequirementType

Converting one code requirement type to another failed because the original requirement included a constraint that is not supported by the target requirement type.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

