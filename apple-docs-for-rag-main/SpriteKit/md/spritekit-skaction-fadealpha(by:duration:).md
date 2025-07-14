

- SpriteKit
- SKAction
-  fadeAlpha(by:duration:) 

Type Method

# fadeAlpha(by:duration:)

Creates an action that adjusts the alpha value of a node by a relative value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func fadeAlpha(
    by factor: CGFloat,
    duration: TimeInterval
) -> SKAction
```

## Parameters 

`factor`  

The amount to add to the node’s alpha value.

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s alpha property animates to its new value.

This action is reversible; the reverse is created as if the following code is executed:

- Swift
- Obj-C

```
let action = SKAction.fadeAlpha(by: -factor, duration: sec)
```

```
[SKAction fadeAlphaBy: -factor duration: sec];
```

## See Also

### Animating the Transparency of a Node

class func fadeIn(withDuration: TimeInterval) -> SKAction

Creates an action that changes the alpha value of the node to `1.0`.

class func fadeOut(withDuration: TimeInterval) -> SKAction

Creates an action that changes the alpha value of the node to `0.0`.

class func fadeAlpha(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that adjusts the alpha value of a node to a new value.

