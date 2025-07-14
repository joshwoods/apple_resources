

- Core Location
- CLLocationPushServiceError
- CLLocationPushServiceError.Code
-  CLLocationPushServiceError.Code.missingPushServerEnvironment 

Case

# CLLocationPushServiceError.Code.missingPushServerEnvironment

An error code that indicates the app is missing an Apple Push Notification service (APNs) environment entitlement.

iOS 15.0+iPadOS 15.0+

``` source
case missingPushServerEnvironment
```

## Discussion

A Location Push Service Extension requires that your app has the APNs environment entitlement. For more information, see APS Environment Entitlement.

## See Also

### Getting the error code

case unknown

An error code that indicates the app was unable to start the location push service for an unknown reason.

case missingPushExtension

An error code that indicates the app is missing a Location Push Service Extension.

case missingEntitlement

An error code that indicates the app is missing the entitlement it needs to use the location push service.

case unsupportedPlatform

An error code that indicates the location push service isn’t available on this platform.

