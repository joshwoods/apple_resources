

- SceneKit
- SCNAction
-  run(\_:) 

Type Method

# run(\_:)

Creates an action that executes a block.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func run(_ block: @escaping (SCNNode) -> Void) -> SCNAction
```

## Parameters 

`block`  

The block to run. The block takes a single parameter:

node  
The node on which the action is running.

## Return Value

A new action object.

## Discussion

When the action executes, SceneKit calls the block. This action takes place instantaneously.

This action is not reversible; the reverse action executes the same block.

## See Also

### Creating Custom Actions

class func run((SCNNode) -> Void, queue: dispatch_queue_t) -> SCNAction

Creates an action that executes a block on a specific dispatch queue.

class func customAction(duration: TimeInterval, action: (SCNNode, CGFloat) -> Void) -> SCNAction

Creates an action that executes a block periodically over a specified duration.

class func javaScriptAction(withScript: String, duration: TimeInterval) -> SCNAction

Creates an action that executes a JavaScript script periodically over a specified duration.

