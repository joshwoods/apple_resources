

- Push to Talk
- PTInstantiationError
-  PTInstantiationError.Code 

Enumeration

# PTInstantiationError.Code

Error codes for instantiation operations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum Code
```

## Topics

### Error codes

case unknown

An instantiation error that indicates an unknown error.

case invalidPlatform

An instantiation error that indicates the API isn’t available on the simulator or macOS devices.

case missingBackgroundMode

An instantiation error that indicates the app doesn’t have the background mode in an enabled state.

case missingPushServerEnvironment

An instantiation error that indicates the app doesn’t have the push notification capability in an enabled state.

case missingEntitlement

An instantiation error that indicates the app is missing the entitlement.

case instantiationAlreadyInProgress

An instantiation error that indicates there’s already an in-flight instantiation request.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Push to Talk errors

struct PTChannelError

A structure that represents a channel error.

enum Code

Error codes for channel operations.

struct PTInstantiationError

A structure that represents an instantiation error.

let PTChannelErrorDomain: String

A string representation of the channel error domain.

let PTInstantiationErrorDomain: String

A string representation of the instantiation error domain.

