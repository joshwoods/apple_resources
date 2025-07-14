

- Core Location
- CLLocationPushServiceError
-  missingPushExtension 

Type Property

# missingPushExtension

An error code that indicates the app is missing a Location Push Service Extension.

iOS 15.0+iPadOS 15.0+

``` source
static var missingPushExtension: CLLocationPushServiceError.Code { get }
```

## See Also

### Getting the error code

static var unknown: CLLocationPushServiceError.Code

An error code that indicates the app was unable to start the location push service for an unknown reason.

static var missingPushServerEnvironment: CLLocationPushServiceError.Code

An error code that indicates the app is missing an Apple Push Notification service (APNs) environment entitlement.

static var missingEntitlement: CLLocationPushServiceError.Code

An error code that indicates the app is missing the entitlement it needs to use the location push service.

static var unsupportedPlatform: CLLocationPushServiceError.Code

An error code that indicates the location push service isn’t available on this platform.

enum Code

Error codes the location manager returns if starting to monitor for location push notifications fails.

