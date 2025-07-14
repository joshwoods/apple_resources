

- SceneKit
- SCNAction
-  customAction(duration:action:) 

Type Method

# customAction(duration:action:)

Creates an action that executes a block periodically over a specified duration.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func customAction(
    duration seconds: TimeInterval,
    action block: @escaping (SCNNode, CGFloat) -> Void
) -> SCNAction
```

## Parameters 

`seconds`  

The duration of the action, in seconds.

`block`  

The block to run. The block takes the following parameters:

*node*  
The node on which the action is running.

*elapsedTime*  
The amount of time that has passed since the action began executing.

## Return Value

A new action object.

## Discussion

When the action executes, SceneKit calls the block repeatedly until the action’s duration expires. For each call, SceneKit computes the elapsed time and passes it to the block.

This action is not reversible; the reverse action executes the same block.

## See Also

### Creating Custom Actions

class func run((SCNNode) -> Void) -> SCNAction

Creates an action that executes a block.

class func run((SCNNode) -> Void, queue: dispatch_queue_t) -> SCNAction

Creates an action that executes a block on a specific dispatch queue.

class func javaScriptAction(withScript: String, duration: TimeInterval) -> SCNAction

Creates an action that executes a JavaScript script periodically over a specified duration.

