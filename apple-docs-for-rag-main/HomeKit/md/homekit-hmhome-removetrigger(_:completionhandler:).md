

- HomeKit
- HMHome
-  removeTrigger(\_:completionHandler:) 

Instance Method

# removeTrigger(\_:completionHandler:)

Removes a trigger from the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func removeTrigger(
    _ trigger: HMTrigger,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func removeTrigger(_ trigger: HMTrigger) async throws
```

## Parameters 

`trigger`  

The trigger to remove.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

If `trigger` is enabled, removing it from the home disables it.

## See Also

### Triggering an action set

var triggers: [HMTrigger]

An array of triggers defined in the home.

func addTrigger(HMTrigger, completionHandler: ((any Error)?) -> Void)

Adds a trigger to the home.

class HMTimerTrigger

A trigger to activate an action set based on a periodic timer.

class HMEventTrigger

A trigger to activate an action set based on a set of events and optional conditions.

class HMTrigger

An abstract base class for triggering actions based on a set of conditions.

