

- SceneKit
- SCNAction
-  scale(to:duration:) 

Type Method

# scale(to:duration:)

Creates an action that uniformly changes the scale factor of a node to an absolute value.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func scale(
    to scale: CGFloat,
    duration sec: TimeInterval
) -> SCNAction
```

## Parameters 

`scale`  

The new value for all three components of the node’s scale.

`sec`  

The duration, in seconds, of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s scale property animates to the new value.

This action is not reversible; the reverse of this action has the same duration but does not change anything.

## See Also

### Creating Actions That Change a Node’s Scale

class func scale(by: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that uniformly changes the scale factor of a node by a relative value.

