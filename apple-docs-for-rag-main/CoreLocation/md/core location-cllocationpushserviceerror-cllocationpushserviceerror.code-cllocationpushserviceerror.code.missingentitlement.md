

- Core Location
- CLLocationPushServiceError
- CLLocationPushServiceError.Code
-  CLLocationPushServiceError.Code.missingEntitlement 

Case

# CLLocationPushServiceError.Code.missingEntitlement

An error code that indicates the app is missing the entitlement it needs to use the location push service.

iOS 15.0+iPadOS 15.0+

``` source
case missingEntitlement
```

## Discussion

For more information, see Creating a location push service extension.

## See Also

### Getting the error code

case unknown

An error code that indicates the app was unable to start the location push service for an unknown reason.

case missingPushExtension

An error code that indicates the app is missing a Location Push Service Extension.

case missingPushServerEnvironment

An error code that indicates the app is missing an Apple Push Notification service (APNs) environment entitlement.

case unsupportedPlatform

An error code that indicates the location push service isn’t available on this platform.

