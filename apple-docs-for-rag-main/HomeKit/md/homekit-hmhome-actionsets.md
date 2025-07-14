

- HomeKit
- HMHome
-  actionSets 

Instance Property

# actionSets

An array of the action sets in the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var actionSets: [HMActionSet] { get }
```

## Discussion

Action sets are instances of HMActionSet.

## See Also

### Creating action sets

func addActionSet(withName: String, completionHandler: (HMActionSet?, (any Error)?) -> Void)

Adds a new action set to the home.

func removeActionSet(HMActionSet, completionHandler: ((any Error)?) -> Void)

Removes an action set from the home.

func executeActionSet(HMActionSet, completionHandler: ((any Error)?) -> Void)

Executes all the actions in a specified action set.

func builtinActionSet(ofType: String) -> HMActionSet?

Retrieves the builtin action set for the specified type.

class HMActionSet

A collection of actions that you trigger as a group.

