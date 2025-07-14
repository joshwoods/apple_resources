

- HomeKit
- HMHome
-  addActionSet(withName:completionHandler:) 

Instance Method

# addActionSet(withName:completionHandler:)

Adds a new action set to the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func addActionSet(
    withName actionSetName: String,
    completionHandler completion: @escaping (HMActionSet?, (any Error)?) -> Void
)
```

``` source
func addActionSet(named actionSetName: String) async throws -> HMActionSet
```

## Parameters 

`actionSetName`  

The name of the new action set. Must not be `nil`, and must not be the name of an action set already in the home.

`completion`  

The block executed after the request is processed.

actionSet  
The newly created action set.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Creating action sets

var actionSets: [HMActionSet]

An array of the action sets in the home.

func removeActionSet(HMActionSet, completionHandler: ((any Error)?) -> Void)

Removes an action set from the home.

func executeActionSet(HMActionSet, completionHandler: ((any Error)?) -> Void)

Executes all the actions in a specified action set.

func builtinActionSet(ofType: String) -> HMActionSet?

Retrieves the builtin action set for the specified type.

class HMActionSet

A collection of actions that you trigger as a group.

