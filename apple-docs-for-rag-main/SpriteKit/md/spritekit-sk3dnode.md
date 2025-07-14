

- SpriteKit
-  SK3DNode 

Class

# SK3DNode

3D SceneKit content drawn as a flattened sprite.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SK3DNode
```

**watchOS**

``` source
class SK3DNode
```

## Mentioned in 

Displaying 3D Content in a SpriteKit Scene

## Overview

Use SK3DNode objects to incorporate 3D SceneKit content into a SpriteKit-based game. When SpriteKit renders the node, the SceneKit scene is animated and rendered first. Then this rendered image is composited into the SpriteKit scene. Use the scnScene property to specify the SceneKit scene to be rendered.

## Topics

### Getting Started with 3D Node

Displaying 3D Content in a SpriteKit Scene

Draw SceneKit content in a SpriteKit scene by using a 3D node.

### Creating 3D Nodes

init(viewportSize: CGSize)

Initializes a new 3D node.

init?(coder: NSCoder)

Tells you when to initialize a 3D node that has been unarchived.

### Configuring a 3D Node

var viewportSize: CGSize

The size of the image rendered by the node.

var scnScene: SCNScene?

The SceneKit scene to render.

var pointOfView: SCNNode?

The Scene Kit node from which the scene’s contents are viewed when rendered.

var autoenablesDefaultLighting: Bool

A Boolean value that determines whether Scene Kit automatically adds lights to a scene.

### Animating a 3D Node’s Content in Scene Kit

var isPlaying: Bool

A Boolean value that determines whether the scene is playing.

var loops: Bool

A Boolean value that determines whether Scene Kit restarts the scene time after all animations in the scene have played.

var sceneTime: TimeInterval

The current scene time.

### Projecting Points and Performing Hit-Testing

func hitTest(CGPoint, options: [String : Any]?) -> [SCNHitTestResult]

Searches the Scene Kit scene for objects corresponding to a point in the rendered image.

func projectPoint(vector_float3) -> vector_float3

Projects a point from the 3D world coordinate system of the SceneKit scene to the 2D viewport coordinate system of the SpriteKit node.

func unprojectPoint(vector_float3) -> vector_float3

Unprojects a point from the SpriteKit node’s 2D viewport coordinate system to the 3D world coordinate system of the SceneKit scene.

## Relationships

### Inherits From

- SKNode

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

