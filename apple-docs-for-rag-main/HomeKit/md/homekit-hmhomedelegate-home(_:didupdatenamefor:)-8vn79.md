

- HomeKit
- HMHomeDelegate
-  home(\_:didUpdateNameFor:) 

Instance Method

# home(\_:didUpdateNameFor:)

Tells the delegate that a home updated the name of a trigger.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
optional func home(
    _ home: HMHome,
    didUpdateNameFor trigger: HMTrigger
)
```

## Parameters 

`home`  

The home.

`trigger`  

The trigger whose name was changed.

## See Also

### Observing Action and Trigger Configuration

func home(HMHome, didAdd: HMActionSet)

Tells the delegate that a home added an action set.

func home(HMHome, didUpdateNameFor: HMActionSet)

Tells the delegate that a home updated the name of an action set.

func home(HMHome, didUpdateActionsFor: HMActionSet)

Tells the delegate that a home updated the actions for an action set.

func home(HMHome, didRemove: HMActionSet)

Tells the delegate that a home removed an action set.

func home(HMHome, didAdd: HMTrigger)

Tells the delegate that a home added a trigger.

func home(HMHome, didUpdate: HMTrigger)

Tells the delegate that a home updated a trigger.

func home(HMHome, didRemove: HMTrigger)

Tells the delegate that a home removed a trigger.

