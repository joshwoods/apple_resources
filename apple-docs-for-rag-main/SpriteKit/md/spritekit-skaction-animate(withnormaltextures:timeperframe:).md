

- SpriteKit
- SKAction
-  animate(withNormalTextures:timePerFrame:) 

Type Method

# animate(withNormalTextures:timePerFrame:)

Creates an action that animates changes to a sprite’s normal texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func animate(
    withNormalTextures textures: [SKTexture],
    timePerFrame sec: TimeInterval
) -> SKAction
```

## Parameters 

`textures`  

An array of textures to use.

`sec`  

The amount of time that each texture is displayed.

## Return Value

A new action object.

## Discussion

This action can only be executed by an SKSpriteNode object. When the action executes, the sprite’s normalTexture property animates through the array of textures. The sprite’s normalTexture property is changed to the next texture in the array. The action then pauses for the specified time before continuing. The action continues until it has finished animating through all of the textures in the array. The total duration of the action is the number of textures multiplied by the frame interval.

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

class func animate(withNormalTextures: [SKTexture], timePerFrame: TimeInterval, resize: Bool, restore: Bool) -> SKAction

Creates an action that animates changes to a sprite’s texture.

class func colorize(with: UIColor, colorBlendFactor: CGFloat, duration: TimeInterval) -> SKAction

Creates an animation that animates a sprite’s color and blend factor.

class func colorize(withColorBlendFactor: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that animates a sprite’s blend factor.

