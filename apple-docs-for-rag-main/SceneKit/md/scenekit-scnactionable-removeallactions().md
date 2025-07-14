

- SceneKit
- SCNActionable
-  removeAllActions() 

Instance Method

# removeAllActions()

Ends and removes all actions from the node.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func removeAllActions()
```

**Required**

## Discussion

When SceneKit removes an action from a node, it skips any remaining animation the action would perform. However, any changes the action has already made to the node’s state remain in effect.

## See Also

### Canceling a Node’s Running Actions

func removeAction(forKey: String)

Removes an action associated with a specific key.

**Required**

