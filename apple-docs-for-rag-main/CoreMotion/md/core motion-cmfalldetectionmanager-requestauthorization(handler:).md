

- Core Motion
- CMFallDetectionManager
-  requestAuthorization(handler:) 

Instance Method

# requestAuthorization(handler:)

Requests authorization to receive notifications about fall detection events.

watchOS 7.2+

``` source
func requestAuthorization(handler: @escaping (CMAuthorizationStatus) -> Void)
```

## Parameters 

`handler`  

A block that is called by the system after the user accepts or declines the authorization request.

The system passes the following parameter:

`status`  
The authorization status chosen by the user.

## Discussion

As soon as the user authorizes fall detection, the system calls the delegate’s fallDetectionManager(_:didDetect:completionHandler:) method and passes the latest fall detection event.

## See Also

### Requesting Authorization

var authorizationStatus: CMAuthorizationStatus

The authorization status for receiving fall detection event notifications.

enum CMAuthorizationStatus

The authorization status for motion-related features.

