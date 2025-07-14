

- HomeKit
- HMTrigger
-  actionSets 

Instance Property

# actionSets

Array of all action sets that will be executed by the trigger.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var actionSets: [HMActionSet] { get }
```

## Discussion

Action sets are instances of HMActionSet.

## See Also

### Managing Action Sets

func addActionSet(HMActionSet, completionHandler: ((any Error)?) -> Void)

Adds an action set to the trigger.

func removeActionSet(HMActionSet, completionHandler: ((any Error)?) -> Void)

Removes an action set from the trigger.

