

- HomeKit
- HMActionSet
-  actions 

Instance Property

# actions

Set of actions in the action set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var actions: Set { get }
```

## See Also

### Defining the associated actions

func addAction(HMAction, completionHandler: HMErrorBlock)

Adds an action to the action set.

func removeAction(HMAction, completionHandler: HMErrorBlock)

Removes an action from the action set.

class HMCharacteristicWriteAction

An action in an action set that writes a value to a characteristic.

class HMAction

An abstract base class for actions in HomeKit.

