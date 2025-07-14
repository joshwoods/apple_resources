

- SceneKit
- SCNActionable
-  runAction(\_:) 

Instance Method

# runAction(\_:)

Adds an action to the list of actions executed by the node.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func runAction(_ action: SCNAction)
```

**Required**

## Parameters 

`action`  

The action to be performed.

## Discussion

SceneKit begins running a newly added action when it prepares to render the next frame.

## See Also

### Running Actions

func runAction(SCNAction, completionHandler: (() -> Void)?)

Adds an action to the list of actions executed by the node. SceneKit calls the specified block when the action completes.

**Required**

func runAction(SCNAction, forKey: String?)

Adds an identifiable action to the list of actions executed by the node.

**Required**

func runAction(SCNAction, forKey: String?, completionHandler: (() -> Void)?)

Adds an identifiable action to the list of actions executed by the node. SceneKit calls the specified block when the action completes.

**Required**

