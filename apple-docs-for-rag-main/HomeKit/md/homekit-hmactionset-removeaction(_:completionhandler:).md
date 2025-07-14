

- HomeKit
- HMActionSet
-  removeAction(\_:completionHandler:) 

Instance Method

# removeAction(\_:completionHandler:)

Removes an action from the action set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func removeAction(
    _ action: HMAction,
    completionHandler completion: @escaping HMErrorBlock
)
```

``` source
func removeAction(_ action: HMAction) async throws
```

## Parameters 

`action`  

The action to remove.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Defining the associated actions

var actions: Set&lt;HMAction>

Set of actions in the action set.

func addAction(HMAction, completionHandler: HMErrorBlock)

Adds an action to the action set.

class HMCharacteristicWriteAction

An action in an action set that writes a value to a characteristic.

class HMAction

An abstract base class for actions in HomeKit.

