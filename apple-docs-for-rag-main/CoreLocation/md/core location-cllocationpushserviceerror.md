

- Core Location
-  CLLocationPushServiceError 

Structure

# CLLocationPushServiceError

Error codes the location manager returns if starting to monitor for location push notifications fails.

iOS 15.0+iPadOS 15.0+

``` source
struct CLLocationPushServiceError
```

## Topics

### Getting the error code

static var unknown: CLLocationPushServiceError.Code

An error code that indicates the app was unable to start the location push service for an unknown reason.

static var missingPushExtension: CLLocationPushServiceError.Code

An error code that indicates the app is missing a Location Push Service Extension.

static var missingPushServerEnvironment: CLLocationPushServiceError.Code

An error code that indicates the app is missing an Apple Push Notification service (APNs) environment entitlement.

static var missingEntitlement: CLLocationPushServiceError.Code

An error code that indicates the app is missing the entitlement it needs to use the location push service.

static var unsupportedPlatform: CLLocationPushServiceError.Code

An error code that indicates the location push service isn’t available on this platform.

enum Code

Error codes the location manager returns if starting to monitor for location push notifications fails.

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

### Location push service extension

com.apple.developer.location.push

An entitlement to enable a location-sharing app to query someone’s location in response to a push notification.

protocol CLLocationPushServiceExtension

The interface you adopt in the type that acts as the main entry point for a Location Push Service Extension.

let CLLocationPushServiceErrorDomain: String

The domain for Location Push Service Extension errors.

enum Code

Error codes the location manager returns if starting to monitor for location push notifications fails.

