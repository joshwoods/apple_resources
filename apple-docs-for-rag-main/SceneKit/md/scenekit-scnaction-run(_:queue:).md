

- SceneKit
- SCNAction
-  run(\_:queue:) 

Type Method

# run(\_:queue:)

Creates an action that executes a block on a specific dispatch queue.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func run(
    _ block: @escaping (SCNNode) -> Void,
    queue: dispatch_queue_t
) -> SCNAction
```

## Parameters 

`block`  

The block to run. The block takes a single parameter:

node  
The node on which the action is running.

`queue`  

The queue to perform the action on.

## Return Value

A new action object.

## Discussion

When the action executes, SceneKit calls the block. This action takes place instantaneously.

This action is not reversible; the reverse action executes the same block.

## See Also

### Creating Custom Actions

class func run((SCNNode) -> Void) -> SCNAction

Creates an action that executes a block.

class func customAction(duration: TimeInterval, action: (SCNNode, CGFloat) -> Void) -> SCNAction

Creates an action that executes a block periodically over a specified duration.

class func javaScriptAction(withScript: String, duration: TimeInterval) -> SCNAction

Creates an action that executes a JavaScript script periodically over a specified duration.

