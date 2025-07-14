

- Media Player
- MPError
-  cancelled 

Type Property

# cancelled

The system cancels the requested operation before it completes.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+macOS 10.14.2+tvOS 10.1+visionOS 1.0+watchOS 5.0+

``` source
static var cancelled: MPError.Code { get }
```

## See Also

### Error code constants

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

