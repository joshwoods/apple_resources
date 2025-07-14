

- SceneKit
- SCNActionable
-  runAction(\_:forKey:) 

Instance Method

# runAction(\_:forKey:)

Adds an identifiable action to the list of actions executed by the node.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func runAction(
    _ action: SCNAction,
    forKey key: String?
)
```

**Required**

## Parameters 

`action`  

The action to be performed.

`key`  

A unique key used to identify the action.

## Discussion

This method is identical to runAction(_:), but the action is stored and identified so that you can retrieve or cancel it later. If an action using the same key is already running, SceneKit removes it before adding the new action.

## See Also

### Related Documentation

func action(forKey: String) -> SCNAction?

Returns an action associated with a specific key.

**Required**

func removeAction(forKey: String)

Removes an action associated with a specific key.

**Required**

### Running Actions

func runAction(SCNAction)

Adds an action to the list of actions executed by the node.

**Required**

func runAction(SCNAction, completionHandler: (() -> Void)?)

Adds an action to the list of actions executed by the node. SceneKit calls the specified block when the action completes.

**Required**

func runAction(SCNAction, forKey: String?, completionHandler: (() -> Void)?)

Adds an identifiable action to the list of actions executed by the node. SceneKit calls the specified block when the action completes.

**Required**

