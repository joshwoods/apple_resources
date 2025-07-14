

- HomeKit
- HMHome
-  triggers 

Instance Property

# triggers

An array of triggers defined in the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var triggers: [HMTrigger] { get }
```

## See Also

### Triggering an action set

func addTrigger(HMTrigger, completionHandler: ((any Error)?) -> Void)

Adds a trigger to the home.

func removeTrigger(HMTrigger, completionHandler: ((any Error)?) -> Void)

Removes a trigger from the home.

class HMTimerTrigger

A trigger to activate an action set based on a periodic timer.

class HMEventTrigger

A trigger to activate an action set based on a set of events and optional conditions.

class HMTrigger

An abstract base class for triggering actions based on a set of conditions.

