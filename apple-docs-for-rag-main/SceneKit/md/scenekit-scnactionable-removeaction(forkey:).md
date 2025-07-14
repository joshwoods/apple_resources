

- SceneKit
- SCNActionable
-  removeAction(forKey:) 

Instance Method

# removeAction(forKey:)

Removes an action associated with a specific key.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func removeAction(forKey key: String)
```

**Required**

## Parameters 

`key`  

A string that uniquely identifies a action.

## Discussion

If the node is currently running an action that matches the key, SceneKit removes that action from the node, skipping any remaining animation it would perform but keeping any changes already made to the node.

Use this method to cancel actions you scheduled using the runAction(_:forKey:) or runAction(_:forKey:completionHandler:) method.

## See Also

### Canceling a Node’s Running Actions

func removeAllActions()

Ends and removes all actions from the node.

**Required**

