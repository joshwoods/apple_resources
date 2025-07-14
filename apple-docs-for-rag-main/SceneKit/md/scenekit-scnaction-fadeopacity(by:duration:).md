

- SceneKit
- SCNAction
-  fadeOpacity(by:duration:) 

Type Method

# fadeOpacity(by:duration:)

Creates an action that adjusts the opacity of a node by a relative value.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func fadeOpacity(
    by factor: CGFloat,
    duration sec: TimeInterval
) -> SCNAction
```

## Parameters 

`factor`  

The amount to change the node’s opacity by.

`sec`  

The duration, in seconds, of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s opacity property animates to its new value.

This action is reversible; the reverse is created as if the following code had been executed:

```
[SCNAction fadeOpacityBy: -factor duration: sec];
```

## See Also

### Creating Actions That Change a Node’s Opacity

class func fadeIn(duration: TimeInterval) -> SCNAction

Creates an action that changes the opacity of the node to `1.0`.

class func fadeOut(duration: TimeInterval) -> SCNAction

Creates an action that changes the opacity of the node to `0.0`.

class func fadeOpacity(to: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that adjusts the opacity of a node to a new value.

