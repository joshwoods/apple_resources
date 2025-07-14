

- HomeKit
- HMHomeManagerDelegate
-  homeManager(\_:didUpdate:) 

Instance Method

# homeManager(\_:didUpdate:)

Tells the delegate when the authorization status changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
optional func homeManager(
    _ manager: HMHomeManager,
    didUpdate status: HMHomeManagerAuthorizationStatus
)
```

## Parameters 

`manager`  

The home manager for which the status changed.

`status`  

The new authorization status. You can also read this value at any time from the manager’s authorizationStatus property.

