

- ManagedApp
-  ManagedAppError 

Enumeration

# ManagedAppError

Errors that functions in the ManagedApp framework can throw.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
enum ManagedAppError
```

## Topics

### Interpreting an error

case invalidIdentifier

An error that indicates a failure finding an identifier.

### Operators

static func == (ManagedAppError, ManagedAppError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case internalError

An error that indicates a failure at the system level.

case serverError

An error that indicates a failure requesting a secret from the asset server.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

## See Also

### Errors

protocol ManagedAppConfigurationDecodingError

A protocol for an error that describes an issue with decoding the configuration.

struct ManagedAppConfigurationDecodingErrorCode

A code for an error that occurs during configuration decoding.

