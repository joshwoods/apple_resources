

- iAd
- ADClient
-  requestAttributionDetails(\_:) Deprecated

Instance Method

# requestAttributionDetails(\_:)

Gets an attribution response.

``` source
func requestAttributionDetails(_ completionHandler: @escaping ([String : NSObject]?, (any Error)?) -> Void)
```

``` source
func requestAttributionDetails() async throws -> [String : NSObject]
```

Deprecated

This has been replaced by functionality in AdServices.framework's AAAttribution class.

## Mentioned in 

Setting Up Apple Search Ads Attribution

iAd Changelog

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

For iOS 14 and later, obtaining an attribution response depends on the calling app’s trackingAuthorizationStatus value and the device-level setting Allow Apps to Request to Track (AAtRtT). The AAtRtT setting allows users to opt in or out of allowing apps to request user consent to access app-related data that third parties can use for both attribution and tracking the user or the device. The following table shows the combination of tracking interactions and expected attribution payload response.

| **Allow Apps to Request to Track setting on a device (iOS 14 and later)** | **Result or ADClientError** | **Authorization Status** |
|----|----|----|
| On | Attribution Response - See Retrieve the Attribution Dictionary | ATTrackingManager.AuthorizationStatus.authorized |
| Off | Attribution Response - See Retrieve the Attribution Dictionary | ATTrackingManager.AuthorizationStatus.authorized |
| On | trackingRestrictedOrDenied | ATTrackingManager.AuthorizationStatus.notDetermined |
| Off | trackingRestrictedOrDenied | ATTrackingManager.AuthorizationStatus.notDetermined |
| On | trackingRestrictedOrDenied | ATTrackingManager.AuthorizationStatus.denied |
| Off | trackingRestrictedOrDenied | ATTrackingManager.AuthorizationStatus.denied |
| Off - the user can’t change the setting. | trackingRestrictedOrDenied | ATTrackingManager.AuthorizationStatus.restricted |

