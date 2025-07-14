

- Distributed
- ExecuteDistributedTargetError
-  ExecuteDistributedTargetError.ErrorCode 

Enumeration

# ExecuteDistributedTargetError.ErrorCode

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
enum ErrorCode
```

## Topics

### Operators

static func == (ExecuteDistributedTargetError.ErrorCode, ExecuteDistributedTargetError.ErrorCode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case invalidGenericSubstitutions

Generic substitutions provided by invocation decoder are incompatible with target of the call. E.g. the generic requirements on the actual target could not be fulfilled by the obtained generic substitutions.

case invalidParameterCount

Call target has different number of parameters than arguments provided by the invocation decoder.

case missingGenericSubstitutions

Target expects generic environment information, but invocation decoder provided no generic substitutions.

case other

A general issue during the execution of the distributed call target occurred.

case targetAccessorNotFound

Unable to resolve the target identifier to a function accessor. This can happen when the identifier is corrupt, illegal, or wrong in the sense that the caller and callee do not have the called function recorded using the same identifier.

case typeDeserializationFailure

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

