

- App Tracking Transparency
- ATTrackingManager
-  requestTrackingAuthorization(completionHandler:) 

Type Method

# requestTrackingAuthorization(completionHandler:)

The request for user authorization to access app-related data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func requestTrackingAuthorization(completionHandler completion: @escaping (ATTrackingManager.AuthorizationStatus) -> Void)
```

``` source
class func requestTrackingAuthorization() async -> ATTrackingManager.AuthorizationStatus
```

## Discussion

The requestTrackingAuthorization(completionHandler:) is a one-time request to authorize or deny access to app-related data that can be used for tracking the user or the device. The system remembers the user’s choice and doesn’t prompt again unless a user uninstalls and then reinstalls the app on the device.

Calls to the API only prompt when the application state is `UIApplicationStateActive`. The authorization prompt doesn’t display if another permission request is pending user confirmation. Concurrent requests aren’t preserved by iOS, and calls to the API through an app extension don’t prompt. Check the trackingAuthorizationStatus for a status of ATTrackingManager.AuthorizationStatus.notDetermined to determine if you need to make an additional call.

The completion handler will be called with the result of the user’s decision for granting or denying permission to use application tracking. The completion handler will be called immediately if access to request authorization is restricted.

Important

To use requestTrackingAuthorization(completionHandler:), the NSUserTrackingUsageDescription key must be in the Information Property List.

