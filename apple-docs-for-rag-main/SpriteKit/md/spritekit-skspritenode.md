

- SpriteKit
-  SKSpriteNode 

Class

# SKSpriteNode

An image or solid color.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
class SKSpriteNode
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKSpriteNode
```

## Mentioned in 

Getting Started with Shape Nodes

Getting Started with Nodes

Animate the Warping of a Sprite

Loading and Using Textures

Adding a Video to a Scene

## Overview

`SKSpriteNode` is an onscreen graphical element that can be initialized from an image or a solid color. SpriteKit adds functionality to its ability to display images using the functions discussed below.

## Topics

### Creating a Sprite from an Image Filename

Start with the basic ways to configure and use a sprite node.

Getting Started with Sprite Nodes

Learn the basics about using images, also known as sprites, with SpriteKit.

convenience init(imageNamed: String)

Initializes a textured sprite using an image file.

convenience init(imageNamed: String, normalMapped: Bool)

Initializes a textured sprite using an image file, optionally adding a normal map to simulate 3D lighting.

### Creating a Sprite from a Texture

Reuse a texture across multiple sprite nodes using initializers or the setter.

convenience init(texture: SKTexture?)

Initializes a textured sprite using an existing texture object.

init(texture: SKTexture?, color: UIColor, size: CGSize)

Initializes a textured sprite in color using an existing texture object.

convenience init(texture: SKTexture?, size: CGSize)

Initializes a textured sprite using an existing texture object but with a specified size.

convenience init(texture: SKTexture?, normalMap: SKTexture?)

Initializes a textured sprite with a normal map to simulate 3D lighting.

var texture: SKTexture?

The texture used to draw the sprite.

### Creating a Solid-Color Sprite

Create a colored block of any size that’s also useful for visual debugging.

convenience init(color: UIColor, size: CGSize)

Initializes a single-color sprite node.

### Initializing a Sprite from an Archive

init?(coder: NSCoder)

Tells you when to initialize a sprite from an archive.

### Setting a Sprite’s Size and Position

Control a sprite’s onscreen placement and size.

Using the Anchor Point to Move a Sprite

Learn how the anchor point affects a sprite’s position.

var size: CGSize

The dimensions of the sprite, in points.

func scale(to: CGSize)

Scales the sprite node to a specified size.

var anchorPoint: CGPoint

Defines the point in the sprite that corresponds to the node’s position.

### Scaling a Sprite in Nine Parts

Resize a sprite in nine parts by defining a center rectangle.

Resizing a Sprite in Nine Parts

Scale a sprite using nine-part algorithm.

var centerRect: CGRect

Enable nine-part stretching of the sprite’s texture.

### Tinting a Sprite

Combine color and blend factor properties to colorize a textured sprite.

Tinting a Sprite

Provide a color and blend factor to additively color your sprite.

var color: UIColor

The sprite’s color.

var colorBlendFactor: CGFloat

A floating-point value that describes how the color is blended with the sprite’s texture.

### Configuring Alpha Blendling

Determine how a sprite uses an alpha value, such as additive blending, that results in the sprite being brighter than it was before.

Blending a Sprite with Different Interpretations of Alpha

Reinterpret a sprite’s alpha property to react differently to the objects below it.

var blendMode: SKBlendMode

The blend mode used to draw the sprite into the parent’s framebuffer.

enum SKBlendMode

The modes that describe how the source and destination pixel colors are used to calculate the new destination color.

### Lighting a Sprite

Configure how a sprite is lit when it’s near a light node.

Lighting a Sprite with Light Nodes

Add lighting and shadows to your scene with light nodes.

var lightingBitMask: UInt32

A mask that defines how this sprite is lit by light nodes in the scene.

var shadowedBitMask: UInt32

A mask that defines which lights add shadows to the sprite.

var shadowCastBitMask: UInt32

A mask that defines which lights are occluded by this sprite.

var normalTexture: SKTexture?

A texture that specifies the normal map for the sprite.

### Adding a Custom Shader to a Sprite

Supply a code file that does custom per-pixel rendering or colorization of a sprite.

Applying Shaders to a Sprite

Write custom GLSL code that modifies the look of your sprite.

var shader: SKShader?

A text file that defines code that does custom per-pixel drawing or colorization.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

Sets the value of a shader attribute.

### Animating a Sprite by Changing its Texture

Animating a Sprite by Changing its Texture

Load a sequence of images and play them back at a rate you define, while optionally looping the resulting animation.

### Instance Properties

var customPlaygroundQuickLook: PlaygroundQuickLook

A custom playground quick look for this instance.

Deprecated

## Relationships

### Inherits From

- SKNode

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- SKWarpable
- Sendable
- UIActivityItemsConfigurationProviding
- UICoordinateSpace
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Nodes that Draw

Maximizing Node Drawing Performance

Structure your nodes for maximum performance.

class SKShapeNode

A mathematical shape that can be stroked or filled.

class SKEmitterNode

A source of various particle effects.

class SKLabelNode

A graphical element that draws text.

class SKVideoNode

A graphical element that plays video content.

class SKTileMapNode

A two-dimensional array of images.

class SK3DNode

3D SceneKit content drawn as a flattened sprite.

