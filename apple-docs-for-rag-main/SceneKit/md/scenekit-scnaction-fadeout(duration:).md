

- SceneKit
- SCNAction
-  fadeOut(duration:) 

Type Method

# fadeOut(duration:)

Creates an action that changes the opacity of the node to `0.0`.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func fadeOut(duration sec: TimeInterval) -> SCNAction
```

## Parameters 

`sec`  

The duration, in seconds, of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s opacity property animates from its current value to `0.0`.

This action is reversible; the reverse is created as if the following code had been executed:

```
[SCNAction fadeInWithDuration: sec];
```

## See Also

### Creating Actions That Change a Node’s Opacity

class func fadeIn(duration: TimeInterval) -> SCNAction

Creates an action that changes the opacity of the node to `1.0`.

class func fadeOpacity(by: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that adjusts the opacity of a node by a relative value.

class func fadeOpacity(to: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that adjusts the opacity of a node to a new value.

