

- SceneKit
- SCNAction
-  fadeOpacity(to:duration:) 

Type Method

# fadeOpacity(to:duration:)

Creates an action that adjusts the opacity of a node to a new value.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func fadeOpacity(
    to opacity: CGFloat,
    duration sec: TimeInterval
) -> SCNAction
```

## Parameters 

`opacity`  

The new opacity value of the node.

`sec`  

The duration, in seconds, of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s opacity property animates to its new value.

This action is not reversible; the reverse of this action has the same duration but does not change anything.

## See Also

### Creating Actions That Change a Node’s Opacity

class func fadeIn(duration: TimeInterval) -> SCNAction

Creates an action that changes the opacity of the node to `1.0`.

class func fadeOut(duration: TimeInterval) -> SCNAction

Creates an action that changes the opacity of the node to `0.0`.

class func fadeOpacity(by: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that adjusts the opacity of a node by a relative value.

