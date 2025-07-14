

- SceneKit
- SCNActionable
-  runAction(\_:completionHandler:) 

Instance Method

# runAction(\_:completionHandler:)

Adds an action to the list of actions executed by the node. SceneKit calls the specified block when the action completes.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func runAction(
    _ action: SCNAction,
    completionHandler block: (() -> Void)? = nil
)
```

``` source
func runAction(_ action: SCNAction) async
```

**Required**

## Parameters 

`action`  

The action to be performed.

`block`  

A completion block that SceneKit calls when the action completes.

## Discussion

Concurrency Note

In Swift, you can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func runAction(_ action: SCNAction) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The new action is processed the next time SceneKit prepares to render a frame.

SceneKit calls your block after the action’s duration is complete. For example, in a game you could use this method to show a Game Over message after performing a fade-out action on a node that displays a player character.

## See Also

### Running Actions

func runAction(SCNAction)

Adds an action to the list of actions executed by the node.

**Required**

func runAction(SCNAction, forKey: String?)

Adds an identifiable action to the list of actions executed by the node.

**Required**

func runAction(SCNAction, forKey: String?, completionHandler: (() -> Void)?)

Adds an identifiable action to the list of actions executed by the node. SceneKit calls the specified block when the action completes.

**Required**

