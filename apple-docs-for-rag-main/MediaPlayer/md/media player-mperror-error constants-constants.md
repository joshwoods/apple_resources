

- Media Player
- MPError
-  Error constants 

API Collection

# Error constants

Error code constants for framework operations.

## Topics

### Error code constants

static var cancelled: MPError.Code

The system cancels the requested operation before it completes.

static var cloudServiceCapabilityMissing: MPError.Code

The operation can’t complete because iCloud services aren’t in an enabled state.

static var unknown: MPError.Code

The requested operation can’t complete due to an unknown error.

static var networkConnectionFailed: MPError.Code

The operation fails because the device can’t connect to the network.

static var notFound: MPError.Code

The operation fails because the system can’t find the requested identifier in the current storefront.

static var notSupported: MPError.Code

The requested operation fails because the system doesn’t support it.

static var permissionDenied: MPError.Code

The operation can’t complete because the user doesn’t have permission for the request.

static var requestTimedOut: MPError.Code

The requested operation times out.

## See Also

### Inspecting an error

enum Code

An enumeration that represents error codes for framework operations.

