

- Core Motion
- CMFallDetectionDelegate
-  fallDetectionManagerDidChangeAuthorization(\_:) 

Instance Method

# fallDetectionManagerDidChangeAuthorization(\_:)

Indicates the fall detection authorization status changed.

watchOS 7.2+

``` source
optional func fallDetectionManagerDidChangeAuthorization(_ fallDetectionManager: CMFallDetectionManager)
```

## Parameters 

`fallDetectionManager`  

The fall detection manager for the event.

## Discussion

The system calls this method after the fall detection authorization status changes. Check the fall detection manager’s authorizationStatus property to determine the current status.

