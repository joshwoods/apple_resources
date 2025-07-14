

- Network Extension
-  NEAppPushManagerError 

Structure

# NEAppPushManagerError

An error that the push manager encounters.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
struct NEAppPushManagerError
```

## Topics

### Inspecting error properties

enum Code

Error codes that the local push API declares.

### Error constants

static var configurationInvalid: NEAppPushManagerError.Code

An error that indicates the app push configuration is invalid.

static var configurationNotLoaded: NEAppPushManagerError.Code

An error that indicates the manager hasn’t loaded the app push configuration.

static var inactiveSession: NEAppPushManagerError.Code

An error that indicates an invalid attempt to perform an operation on an inactive session.

static var internalError: NEAppPushManagerError.Code

An error that indicates an internal error in the local push connectivity framework.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Handling errors

let NEAppPushErrorDomain: String

The error domain string for local push errors.

enum Code

Error codes that the local push API declares.

