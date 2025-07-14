

- SpriteKit
- SKAction
-  animate(withNormalTextures:timePerFrame:resize:restore:) 

Type Method

# animate(withNormalTextures:timePerFrame:resize:restore:)

Creates an action that animates changes to a sprite’s texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func animate(
    withNormalTextures textures: [SKTexture],
    timePerFrame sec: TimeInterval,
    resize: Bool,
    restore: Bool
) -> SKAction
```

## Parameters 

`textures`  

An array of textures to use when animating a sprite.

`sec`  

The amount of time that each texture is displayed.

`resize`  

If true, the sprite is resized to match each new texture. If false, the size of the sprite remains at a constant size.

`restore`  

- If true:

When the action completes, the sprite’s texture is restored to the texture it had before the action completed. (If the resize parameter is true, the sprite is resized to match the size of the original texture.)

- If false:

When the action completes, the sprite’s texture remains set to the final texture in the array.

## Return Value

A new action object.

## Discussion

This action can only be executed by an SKSpriteNode object. When the action executes, the sprite’s normalTexture property animates through the array of textures. The sprite’s normalTexture property is changed to the next texture in the array. The action then pauses for the specified time before continuing. The action continues until it has finished animating through all of the textures in the array. The total duration of the action is the number of textures multiplied by the frame interval.

Note

If the `restore` parameter is true and this action is removed from a node before it completes, then node’s normal texture is still restored. This differs from the default behavior of removing an action.

This action is reversible; the resulting action animates through the same textures from last to first.

## See Also

### Animating a Node’s Texture

class func resize(byWidth: CGFloat, height: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that adjusts the size of a sprite.

class func resize(toHeight: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the height of a sprite to a new absolute value.

class func resize(toWidth: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the width of a sprite to a new absolute value.

class func resize(toWidth: CGFloat, height: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the width and height of a sprite to a new absolute value.

class func setTexture(SKTexture) -> SKAction

Creates an action that changes a sprite’s texture.

class func setTexture(SKTexture, resize: Bool) -> SKAction

Creates an action that changes a sprite’s texture, possibly resizing the sprite.

class func animate(with: [SKTexture], timePerFrame: TimeInterval) -> SKAction

Creates an action that animates changes to a sprite’s texture.

class func animate(with: [SKTexture], timePerFrame: TimeInterval, resize: Bool, restore: Bool) -> SKAction

Creates an action that animates changes to a sprite’s texture, possibly resizing the sprite.

class func setNormalTexture(SKTexture) -> SKAction

Creates an action that changes a sprite’s normal texture.

class func setNormalTexture(SKTexture, resize: Bool) -> SKAction

Creates an action that changes a sprite’s normal texture, possibly resizing the sprite.

class func animate(withNormalTextures: [SKTexture], timePerFrame: TimeInterval) -> SKAction

Creates an action that animates changes to a sprite’s normal texture.

class func colorize(with: UIColor, colorBlendFactor: CGFloat, duration: TimeInterval) -> SKAction

Creates an animation that animates a sprite’s color and blend factor.

class func colorize(withColorBlendFactor: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that animates a sprite’s blend factor.

