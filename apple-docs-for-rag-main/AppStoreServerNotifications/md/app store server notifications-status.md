

- App Store Server Notifications
-  status 

Type

# status

The status of an auto-renewable subscription at the time the App Store signs the notification.

App Store Server Notifications 2.8+

``` source
int32 status
```

## Possible Values 

`1`  

The auto-renewable subscription is active.

`2`  

The auto-renewable subscription is expired.

`3`  

The auto-renewable subscription is in a billing retry period.

`4`  

The auto-renewable subscription is in a Billing Grace Period.

`5`  

The auto-renewable subscription is revoked.

## Mentioned in 

App Store Server Notifications changelog

## Discussion

This status value is current as of the `signedDate` in the decoded payload, responseBodyV2DecodedPayload.

## See Also

### App metadata and environment

type appAppleId

The unique identifier of an app in the App Store.

type bundleId

The bundle identifier of an app.

type bundleVersion

The version of the build that identifies an iteration of the bundle.

type environment

The server environment, either sandbox or production.

