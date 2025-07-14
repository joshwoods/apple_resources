

- SpriteKit
-  SKEffectNode 

Class

# SKEffectNode

A node that renders its children into a separate buffer, optionally applying an effect, before drawing the final result.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKEffectNode
```

**watchOS**

``` source
class SKEffectNode
```

## Mentioned in 

Creating a New Node By Rendering To a Texture

About Node Drawing Order

Warping SpriteKit Content By Using an Effect Node

Adding a Video to a Scene

Animate the Warping of a Sprite

## Overview

An SKEffectNode object renders its children into a buffer and optionally applies a Core Image filter to this rendered output. Because effect nodes conform to SKWarpable, you can also use them to apply distortions to nodes that don’t implement the protocol, such as shape and video nodes. Use effect nodes to incorporate sophisticated special effects into a scene or to cache the contents of a static subtree for faster rendering performance.

Each time a new frame is rendered using the effect node, the effect node follows these steps:

1.  It draws its children into a private framebuffer.

2.  It applies a Core Image effect to the private framebuffer. This stage is optional; see the filter and shouldEnableEffects properties.

3.  It blends the contents of its private framebuffer into its parent’s framebuffer, using one of the standard sprite blend modes.

4.  It discards its private framebuffer. This step is optional; see the shouldRasterize property.

## Topics

### Applying Core Image Filters with an Effect Node

Applying Special Effects to a Node’s Children

Apply the Core Image suite of filters to child nodes of an effect node.

var filter: CIFilter?

The Core Image filter to apply.

var shouldEnableEffects: Bool

A Boolean value that determines whether the effect node applies the filter to its children as they are drawn.

var shouldCenterFilter: Bool

A Boolean value that determines whether the effect node automatically sets the filter’s image center.

### Warping Nodes with an Effect Node

Warping SpriteKit Content By Using an Effect Node

Distort the child nodes of an effect node by applying a warping effect.

### Applying a Shader with an Effect Node

Supply a code file that does custom per-pixel alteration or colorization of an effect node’s children.

var shader: SKShader?

A custom shader that is called when the effect node is blended into the parent’s framebuffer.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

Gets the value of a shader attribute.

### Flattening an Effect Node’s Child Tree for Performance Improvement

Improving the Performance of Static Content

Flatten a portion of your node hierarchy to a single texture to improve performance.

var shouldRasterize: Bool

A Boolean value that indicates whether the results of rendering the child nodes should be cached.

### Configuring Alpha Blending

Change how an effect node uses its alpha value, such as additive blending, that results in the sprite being brighter than it was before.

var blendMode: SKBlendMode

The blend mode used to draw the node’s contents into its parent’s framebuffer.

## Relationships

### Inherits From

- SKNode

### Inherited By

- SKScene

### Conforms To

- CVarArg
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

### Nodes that Modify Drawing

class SKCropNode

A node that masks pixels drawn by its children so that only some pixels are seen.

class SKTransformNode

A node that allows its children to rotate in 3D.

