

- HomeKit
- HMActionSet
-  addAction(\_:completionHandler:) 

Instance Method

# addAction(\_:completionHandler:)

Adds an action to the action set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func addAction(
    _ action: HMAction,
    completionHandler completion: @escaping HMErrorBlock
)
```

``` source
func addAction(_ action: HMAction) async throws
```

## Parameters 

`action`  

The action to add. Actions may only be in one set—create separate HMAction objects for the same conceptual action if you want an action to be in more than one action set.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Defining the associated actions

var actions: Set&lt;HMAction>

Set of actions in the action set.

func removeAction(HMAction, completionHandler: HMErrorBlock)

Removes an action from the action set.

class HMCharacteristicWriteAction

An action in an action set that writes a value to a characteristic.

class HMAction

An abstract base class for actions in HomeKit.

