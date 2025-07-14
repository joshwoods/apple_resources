

- Push to Talk
- PTChannelError
-  PTChannelError.Code 

Enumeration

# PTChannelError.Code

Error codes for channel operations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum Code
```

## Mentioned in 

Creating a Push to Talk app

## Topics

### Error codes

case unknown

A channel error that indicates an unknown error.

case appNotForeground

A channel error that indicates the operation failed because the app isn’t in the foreground.

case channelNotFound

A channel error that indicates the system can’t perform the action because there’s no active channel with the UUID you specify.

case channelLimitReached

A channel error that indicates you reached the maximum of one active channel at a time for the entire device.

case callActive

A channel error that indicates there’s an active call that prevents the channel action.

case transmissionInProgress

A channel error that indicates a transmission is already in progress.

case transmissionNotFound

A channel error that indicates there’s no transmission to stop.

case deviceManagementRestriction

A channel error that indicates a device-management policy or profile forbids joining the channel.

case screenTimeRestriction

A channel error that indicates a Screen Time restriction prevents the action.

case transmissionNotAllowed

A channel error that indicates the current transmission mode of the channel doesn’t allow the mode you specify.

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

struct PTInstantiationError

A structure that represents an instantiation error.

enum Code

Error codes for instantiation operations.

let PTChannelErrorDomain: String

A string representation of the channel error domain.

let PTInstantiationErrorDomain: String

A string representation of the instantiation error domain.

