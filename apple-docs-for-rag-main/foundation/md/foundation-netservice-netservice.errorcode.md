

- Foundation
- NetService
-  NetService.ErrorCode 

Enumeration

# NetService.ErrorCode

These constants identify errors that can occur when accessing net services.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
enum ErrorCode
```

## Topics

### Constants

case unknownError

An unknown error occurred.

case collisionError

The service could not be published because the name is already in use. The name could be in use locally or on another system.

case notFoundError

The service could not be found on the network.

case activityInProgress

The net service cannot process the request at this time. No additional information about the network state is known.

case badArgumentError

An invalid argument was used when creating the `NSNetService` object.

case cancelledError

The client canceled the action.

case invalidError

The net service was improperly configured.

case timeoutError

The net service has timed out.

case unknownError

An unknown error occurred.

case collisionError

The service could not be published because the name is already in use. The name could be in use locally or on another system.

case notFoundError

The service could not be found on the network.

case activityInProgress

The net service cannot process the request at this time. No additional information about the network state is known.

case badArgumentError

An invalid argument was used when creating the `NSNetService` object.

case cancelledError

The client canceled the action.

case invalidError

The net service was improperly configured.

case timeoutError

The net service has timed out.

### Enumeration Cases

case missingRequiredConfigurationError

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

### Constants

NSNetServices Errors

If an error occurs, the delegate error-handling methods return a dictionary with the following keys.

struct Options

These constants specify options for a network service.

