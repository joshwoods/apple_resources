

- SpriteKit
- SKAction
-  setTexture(\_:) 

Type Method

# setTexture(\_:)

Creates an action that changes a sprite’s texture.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.10+tvOS 7.1+visionOS 1.0+watchOS 1.0+

``` source
class func setTexture(_ texture: SKTexture) -> SKAction
```

## Parameters 

`texture`  

The new texture to use on the sprite.

## Return Value

A new action object.

## Discussion

This action can only be executed by an SKSpriteNode object. When the action executes, the sprite’s texture property changes immediately to the new texture.

This action is not reversible; the reverse of this action does nothing.

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

class func animate(withNormalTextures: [SKTexture], timePerFrame: TimeInterval, resize: Bool, restore: Bool) -> SKAction

Creates an action that animates changes to a sprite’s texture.

class func colorize(with: UIColor, colorBlendFactor: CGFloat, duration: TimeInterval) -> SKAction

Creates an animation that animates a sprite’s color and blend factor.

class func colorize(withColorBlendFactor: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that animates a sprite’s blend factor.

