

- SpriteKit
- SKAction
-  fadeOut(withDuration:) 

Type Method

# fadeOut(withDuration:)

Creates an action that changes the alpha value of the node to `0.0`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func fadeOut(withDuration duration: TimeInterval) -> SKAction
```

## Parameters 

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Mentioned in 

Getting Started with Actions

## Discussion

When the action executes, the node’s alpha property animates from its current value to `0.0`. This causes the node to disappear.

This action is reversible; the reverse is created as if the following code is executed:

- Swift
- Obj-C

```
let action = SKAction.fadeIn(withDuration: sec)
```

```
[SKAction fadeInWithDuration: sec];
```

## See Also

### Animating the Transparency of a Node

class func fadeIn(withDuration: TimeInterval) -> SKAction

Creates an action that changes the alpha value of the node to `1.0`.

class func fadeAlpha(by: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that adjusts the alpha value of a node by a relative value.

class func fadeAlpha(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that adjusts the alpha value of a node to a new value.

