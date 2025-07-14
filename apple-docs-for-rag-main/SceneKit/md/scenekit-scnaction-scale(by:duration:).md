

- SceneKit
- SCNAction
-  scale(by:duration:) 

Type Method

# scale(by:duration:)

Creates an action that uniformly changes the scale factor of a node by a relative value.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func scale(
    by scale: CGFloat,
    duration sec: TimeInterval
) -> SCNAction
```

## Parameters 

`scale`  

The amount of change to make to all three components of the node’s scale.

`sec`  

The duration, in seconds, of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s scale property animates to the new value.

This action is reversible; the reverse is created as if the following code had been executed:

```
[SCNAction scaleBy: -scale duration: sec];
```

## See Also

### Creating Actions That Change a Node’s Scale

class func scale(to: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that uniformly changes the scale factor of a node to an absolute value.

