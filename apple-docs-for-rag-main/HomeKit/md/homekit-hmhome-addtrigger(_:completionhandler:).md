

- HomeKit
- HMHome
-  addTrigger(\_:completionHandler:) 

Instance Method

# addTrigger(\_:completionHandler:)

Adds a trigger to the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func addTrigger(
    _ trigger: HMTrigger,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func addTrigger(_ trigger: HMTrigger) async throws
```

## Parameters 

`trigger`  

The name of the new trigger. Must not be `nil`, and must not be the name of a trigger already in the home.

`completion`  

The block executed after the request is processed.

trigger  
The newly created trigger.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Triggering an action set

var triggers: [HMTrigger]

An array of triggers defined in the home.

func removeTrigger(HMTrigger, completionHandler: ((any Error)?) -> Void)

Removes a trigger from the home.

class HMTimerTrigger

A trigger to activate an action set based on a periodic timer.

class HMEventTrigger

A trigger to activate an action set based on a set of events and optional conditions.

class HMTrigger

An abstract base class for triggering actions based on a set of conditions.

