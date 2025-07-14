

- SpriteKit
- SKAction
-  speed(by:duration:) 

Type Method

# speed(by:duration:)

Creates an action that changes how fast the node executes actions by a relative value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func speed(
    by speed: CGFloat,
    duration: TimeInterval
) -> SKAction
```

## Parameters 

`speed`  

The amount to add to the node’s speed.

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s speed property animates to the new value.

This action is reversible; the reverse is created as if the following code is executed:

- Swift
- Obj-C

```
let action = SKAction.speed(by: -speed, duration: sec)
```

```
[SKAction speedBy: -speed duration: sec];
```

## See Also

### Controlling the Action’s Speed

class func speed(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes how fast the node executes actions.

