

- HomeKit
- HMHome
-  builtinActionSet(ofType:) 

Instance Method

# builtinActionSet(ofType:)

Retrieves the builtin action set for the specified type.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func builtinActionSet(ofType actionSetType: String) -> HMActionSet?
```

## Parameters 

`actionSetType`  

Type of the builtin action set. Supported action set types are HMActionSetTypeWakeUp, HMActionSetTypeSleep, HMActionSetTypeHomeDeparture and HMActionSetTypeHomeArrival.

## Return Value

The builtin action set corresponding to the type argument.

## Discussion

Returns `nil` if no action set is found.

## See Also

### Creating action sets

var actionSets: [HMActionSet]

An array of the action sets in the home.

func addActionSet(withName: String, completionHandler: (HMActionSet?, (any Error)?) -> Void)

Adds a new action set to the home.

func removeActionSet(HMActionSet, completionHandler: ((any Error)?) -> Void)

Removes an action set from the home.

func executeActionSet(HMActionSet, completionHandler: ((any Error)?) -> Void)

Executes all the actions in a specified action set.

class HMActionSet

A collection of actions that you trigger as a group.

