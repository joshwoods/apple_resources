

- SpriteKit
-  SKShapeNode 

Class

# SKShapeNode

A mathematical shape that can be stroked or filled.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
class SKShapeNode
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKShapeNode
```

## Mentioned in 

Animate the Warping of a Sprite

Creating a Shape Node from an Array of Points

Getting Started with Shape Nodes

## Overview

`SKShapeNode` allows you to create onscreen graphical elements from mathematical points, lines, and curves. The advantage this has over rasterized graphics, such as those displayed by textures, is that shapes are rasterized dynamically at runtime to produce crisp detail and smoother edges.

## Topics

### First Steps

Getting Started with Shape Nodes

Create a filled or stroked shape from a path object.

### Creating a Shape from a Path

convenience init(path: CGPath)

Creates a shape node from a Core Graphics path.

convenience init(path: CGPath, centered: Bool)

Creates a shape node from a Core Graphics path, centered around its position.

var path: CGPath?

The path that defines the shape.

### Creating a Shape from a Rectangle

convenience init(rect: CGRect)

Creates a shape node with a rectangular path.

convenience init(rectOf: CGSize)

Creates a shape node with a rectangular path centered on the node’s origin.

convenience init(rect: CGRect, cornerRadius: CGFloat)

Creates a shape with a rectangular path that has rounded corners.

convenience init(rectOf: CGSize, cornerRadius: CGFloat)

Creates a shape with a rectangular path that has rounded corners centered on the node’s position.

### Creating a Circle Shape

convenience init(circleOfRadius: CGFloat)

Creates a shape node with a circular path centered on the node’s origin.

### Creating an Ellipse Shape

convenience init(ellipseOf: CGSize)

Creates a shape node with an elliptical path centered on the node’s origin.

convenience init(ellipseIn: CGRect)

Creates a shape node with an elliptical path that fills the specified rectangle.

### Creating a Shape from an Array of Points

Creating a Shape Node from an Array of Points

Create jagged or smooth shapes from the same array of points.

convenience init(points: UnsafeMutablePointer&lt;CGPoint>, count: Int)

Creates a shape node from a series of points.

convenience init(splinePoints: UnsafeMutablePointer&lt;CGPoint>, count: Int)

Creates a shape node from a series of spline points.

### Filling a Shape

var fillColor: UIColor

The color used to fill the shape.

var fillTexture: SKTexture?

The texture used to fill the shape.

### Stroking a Shape

var lineWidth: CGFloat

The width used to stroke the path.

var strokeColor: UIColor

The color used to stroke the shape.

var strokeTexture: SKTexture?

The texture used to stroke the shape.

var glowWidth: CGFloat

A glow that extends outward from the stroked line.

var lineCap: CGLineCap

The style used to render the endpoints of the stroked portion of the shape node.

var lineJoin: CGLineJoin

The junction type used when the stroked portion of the shape node is rendered.

var miterLimit: CGFloat

The miter limit to use when the line is stroked using a miter join style.

var isAntialiased: Bool

A Boolean value that determines whether the stroked path is smoothed when drawn.

### Configuring Alpha Blending

Change how a shape uses its alpha value, such as additive blending, that results in the shape being brighter than it was before.

var blendMode: SKBlendMode

The blend mode used to blend the shape into the parent’s framebuffer.

### Controlling or Animating Sroke Length

Adjust or animate a shape’s stroke.

var lineLength: CGFloat

The length of the line defined by the shape node.

### Customizing Stroking or Fill Drawing

Take per-pixel control of drawing the stroke or fill by supplying a custom code file.

Controlling Shape Drawing with Shaders

Change a shape node’s appearance by supplying custom shader code.

var strokeShader: SKShader?

A custom shader used to determine the color of the stroked portion of the shape node.

var fillShader: SKShader?

A custom shader used to determine the color of the filled portion of the shape node.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

The value of a shader attribute.

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

class SKSpriteNode

An image or solid color.

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

