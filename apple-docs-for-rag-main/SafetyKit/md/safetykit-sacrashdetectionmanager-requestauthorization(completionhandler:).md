

- SafetyKit
- SACrashDetectionManager
-  requestAuthorization(completionHandler:) 

Instance Method

# requestAuthorization(completionHandler:)

Requests permission to access Crash Detection information.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
func requestAuthorization(completionHandler handler: @escaping (SAAuthorizationStatus, (any Error)?) -> Void)
```

``` source
func requestAuthorization() async throws -> SAAuthorizationStatus
```

## Parameters 

`handler`  

The completion handler invoked with the status of the authorization request.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method requests a person to authorize your app to receive Crash Detection events. Before requesting authorization, verify that your app already has authorization by verifying that authorizationStatus is true.

## See Also

### Requesting authorization

var delegate: (any SACrashDetectionDelegate)?

The object that receives Crash Detection events.

