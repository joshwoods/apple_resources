

- Core Location
- CLLocationPushServiceExtension
-  didReceiveLocationPushPayload(\_:completion:) 

Instance Method

# didReceiveLocationPushPayload(\_:completion:)

Delivers a location push notification for your app extension to process.

iOS 15.0+iPadOS 15.0+

``` source
func didReceiveLocationPushPayload(
    _ payload: [String : Any],
    completion: @escaping () -> Void
)
```

``` source
func didReceiveLocationPushPayload(_ payload: [String : Any]) async
```

**Required**

## Parameters 

`payload`  

The payload containing the location push.

`completion`  

The block to execute after you receive and process the device’s location. This block has no return value and no parameters.

Execute this block as quickly as possible after you finish the location-related task. If you take too long to execute this block, the system calls the serviceExtensionWillTerminate() method as a warning. If you still don’t call the block in a timely manner, the system terminates your app extension.

## Mentioned in 

Creating a location push service extension

## Discussion

Important

You can implement this delegate method as a synchronous method that takes a completion handler, as shown on this page, or as an asynchronous method that has the following declaration:

```
func didReceiveLocationPushPayload(_ payload: [String : Any]) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

When the system receives a location push notification that targets your app, it runs your app extension and calls this method. Use your implementation of this method to request the device’s current location and do something with that information. For example, a location-sharing app might send the location back to a server to update the person’s current location.

When you add a location push service app extension to your project, the Xcode template includes an implementation of this method for you to modify. The template uses this method to store the completion block and initialize a CLLocationManager instance. Process the result of your location query in the CLLocationManagerDelegate methods.

Important

Protecting user privacy is important when handling location data. End-to-end encryption provides enhanced security if your app moves location data off the user’s device, including transmitting it to a server or to another user. For more information, see Protecting the User’s Privacy.

Store the completion block and call it after you finish processing the location request. Also call the completion block when the system calls serviceExtensionWillTerminate().

