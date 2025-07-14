

- SceneKit
- SCNActionable
-  runAction(\_:forKey:completionHandler:) 

Instance Method

# runAction(\_:forKey:completionHandler:)

Adds an identifiable action to the list of actions executed by the node. SceneKit calls the specified block when the action completes.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func runAction(
    _ action: SCNAction,
    forKey key: String?,
    completionHandler block: (() -> Void)? = nil
)
```

``` source
func runAction(
    _ action: SCNAction,
    forKey key: String?
) async
```

**Required**

## Parameters 

`action`  

The action to be performed.

`key`  

A unique key used to identify the action.

`block`  

A completion block called when the action completes.

## Discussion

Concurrency Note

In Swift, you can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func runAction(_ action: SCNAction, forKey key: String?) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method is identical to runAction(_:completionHandler:), but the action is stored and identified so that you can retrieve or cancel it later. If an action using the same key is already running, SceneKit removes it before adding the new action.

SceneKit calls your block after the action’s duration is complete. For example, you can use this method with a wait action to execute some code after a timed delay. If during the delay period you need to prevent the code from running, use the removeAction(forKey:) method to cancel it.

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

func runAction(SCNAction, forKey: String?)

Adds an identifiable action to the list of actions executed by the node.

**Required**

