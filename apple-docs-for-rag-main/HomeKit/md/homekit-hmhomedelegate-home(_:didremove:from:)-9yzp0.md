

- HomeKit
- HMHomeDelegate
-  home(\_:didRemove:from:) 

Instance Method

# home(\_:didRemove:from:)

Tells the delegate that a home removed a service from a service group.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
optional func home(
    _ home: HMHome,
    didRemove service: HMService,
    from group: HMServiceGroup
)
```

## Parameters 

`home`  

The home.

`service`  

The service that was removed.

`group`  

The group from which the service was removed.

## See Also

### Observing Service Configuration

func home(HMHome, didAdd: HMServiceGroup)

Tells the delegate that a home added a service group.

func home(HMHome, didUpdateNameFor: HMServiceGroup)

Tells the delegate that a home updated the name of a service group.

func home(HMHome, didAdd: HMService, to: HMServiceGroup)

Tells the delegate that a home added a service to a service group.

func home(HMHome, didRemove: HMServiceGroup)

Tells the delegate that a home removed a service group.

