

- Media Player
- MPError
-  notSupported 

Type Property

# notSupported

The requested operation fails because the system doesn’t support it.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.14.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
static var notSupported: MPError.Code { get }
```

## Discussion

An example of this is trying to add a media item to a smart playlist.

## See Also

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

static var permissionDenied: MPError.Code

The operation can’t complete because the user doesn’t have permission for the request.

static var requestTimedOut: MPError.Code

The requested operation times out.

