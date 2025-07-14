

- HomeKit
- HMHome
-  removeActionSet(\_:completionHandler:) 

Instance Method

# removeActionSet(\_:completionHandler:)

Removes an action set from the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func removeActionSet(
    _ actionSet: HMActionSet,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func removeActionSet(_ actionSet: HMActionSet) async throws
```

## Parameters 

`actionSet`  

The action set to remove.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Creating action sets

var actionSets: [HMActionSet]

An array of the action sets in the home.

func addActionSet(withName: String, completionHandler: (HMActionSet?, (any Error)?) -> Void)

Adds a new action set to the home.

func executeActionSet(HMActionSet, completionHandler: ((any Error)?) -> Void)

Executes all the actions in a specified action set.

func builtinActionSet(ofType: String) -> HMActionSet?

Retrieves the builtin action set for the specified type.

class HMActionSet

A collection of actions that you trigger as a group.

