

- HomeKit
- HMHomeDelegate
-  home(\_:didAdd:) 

Instance Method

# home(\_:didAdd:)

Tells the delegate that a home added a service group.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
optional func home(
    _ home: HMHome,
    didAdd group: HMServiceGroup
)
```

## Parameters 

`home`  

The home.

`group`  

The new service group.

## See Also

### Observing Service Configuration

func home(HMHome, didUpdateNameFor: HMServiceGroup)

Tells the delegate that a home updated the name of a service group.

func home(HMHome, didAdd: HMService, to: HMServiceGroup)

Tells the delegate that a home added a service to a service group.

func home(HMHome, didRemove: HMService, from: HMServiceGroup)

Tells the delegate that a home removed a service from a service group.

func home(HMHome, didRemove: HMServiceGroup)

Tells the delegate that a home removed a service group.

