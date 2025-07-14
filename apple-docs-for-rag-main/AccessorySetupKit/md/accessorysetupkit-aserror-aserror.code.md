

- AccessorySetupKit
- ASError
-  ASError.Code 

Enumeration

# ASError.Code

Codes that describe errors encountered during accessory discovery.

iOS 18.0+iPadOS 18.0+

``` source
enum Code
```

## Topics

### Creating an error code

init?(rawValue: Int)

### Activation errors

case activationFailed

Session activation failed.

### Timeout and life cycle errors

case discoveryTimeout

Accessory discovery timed out.

case invalidated

The session invalidated prior to completing the operation.

### Configuration errors

case extensionNotFound

The framework couldn’t find the app extension.

case userRestricted

The person using the app restricted access.

case invalidRequest

The session received an invalid request.

### Picker errors

case pickerRestricted

The picker can’t be used because the app is in the background.

case pickerAlreadyActive

The picker received a show request when it was already active.

### Cancellation errors

case userCancelled

The person using the app canceled the operation.

### Communication errors

case connectionFailed

The session was unable to establish a connection.

### Success cases

case success

A code that represents a successful action.

### Unclassified errors

case unknown

An underlying failure with an unknown cause.

### Accessing the error domain

static var errorDomain: String

The domain of the error.

let ASErrorDomain: String

NSError domain for AccessorySetupKit errors.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct ASError

An error encountered during accessory discovery.

let ASErrorDomain: String

NSError domain for AccessorySetupKit errors.

