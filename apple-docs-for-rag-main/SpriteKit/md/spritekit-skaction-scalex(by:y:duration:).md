

- SpriteKit
- SKAction
-  scaleX(by:y:duration:) 

Type Method

# scaleX(by:y:duration:)

Creates an action that adds relative values to the x and y scale values of a node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func scaleX(
    by xScale: CGFloat,
    y yScale: CGFloat,
    duration: TimeInterval
) -> SKAction
```

## Parameters 

`xScale`  

The amount to add to the node’s x scale value.

`yScale`  

The amount to add to the node’s y scale value.

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s xScale and yScale properties are animated to the new value.

This action is reversible; the reverse is created as if the following code is executed:

- Swift
- Obj-C

```
let action = SKAction.scaleX(by: -scaleX, y: -scaleY, duration: sec)
```

```
[SKAction scaleXBy: -xScale y: -yScale duration: sec];
```

## See Also

### Animating the Scaling of a Node

class func scale(by: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the x and y scale values of a node by a relative value.

class func scale(to: CGSize, duration: TimeInterval) -> SKAction

Creates an action that changes the x and y scale values of a node to achieve

class func scale(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the x and y scale values of a node.

class func scaleX(to: CGFloat, y: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the x and y scale values of a node.

class func scaleX(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the x scale value of a node to a new value.

class func scaleY(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the y scale value of a node to a new value.

