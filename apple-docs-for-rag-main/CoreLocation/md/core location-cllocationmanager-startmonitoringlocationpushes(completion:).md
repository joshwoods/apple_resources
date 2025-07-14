

- Core Location
- CLLocationManager
-  startMonitoringLocationPushes(completion:) 

Instance Method

# startMonitoringLocationPushes(completion:)

Starts monitoring for the delivery of Apple Push Notification service (APNs) location pushes, and provides a device-specific token for sending pushes.

iOS 15.0+iPadOS 15.0+

``` source
func startMonitoringLocationPushes(completion: ((Data?, (any Error)?) -> Void)? = nil)
```

``` source
func startMonitoringLocationPushes() async throws -> Data
```

## Parameters 

`completion`  

The completion handler to call after you start monitoring location pushes. The completion handler takes the following parameters:

`token`  
A globally unique token that identifies this device to APNs. Send this `token` to the server that you use to generate location pushes. Your server passes this `token` — unmodified — back to APNs when sending pushes. APNs device tokens are of variable length. Don’t hard-code their size.

If an error occurs, `token` is `nil`.

`error`  
If your app is unable to register for location pushes, the system sets this parameter to an error object that contains information about why it failed; otherwise it’s `nil`. The error type is CLLocationPushServiceError.

## Mentioned in 

Creating a location push service extension

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func startMonitoringLocationPushes() async throws -> Data
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This function requests an Apple Push Notification service (APNs) token that the system uses to launch your Location Push Service Extension and deliver pushes. Devices need an Internet connection to receive the token. Your completion block receives the token if the call succeeds, otherwise it receives error information. If a compatible iPad or iPhone app calls this method when running in visionOS, the method does nothing.

To use location push notifications, your app must have the `com.apple.developer.location.push` entitlement. For more information about implementing location pushes in your app, see Creating a location push service extension.

## See Also

### Monitoring location push notifications

func stopMonitoringLocationPushes()

Stops monitoring for Apple Push Notification service (APNs) location pushes.

