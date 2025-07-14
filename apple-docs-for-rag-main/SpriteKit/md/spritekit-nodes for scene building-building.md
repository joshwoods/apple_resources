

- SpriteKit
-  Nodes for Scene Building 

API Collection

# Nodes for Scene Building

Define the appearance or layout of scene content.

## Topics

### Base Nodes

Provide a reference, point of view, or foundation to all things displayed in a scene.

Using Base Nodes to Lay Out SpriteKit Content

Use nonvisual nodes to define the layout of a scene.

class SKNode

The base class of all SpriteKit nodes.

class SKCameraNode

A node that determines which parts of the scene are visible within a view.

class SKReferenceNode

A node that’s defined in an archived `.sks` file.

### Nodes that Draw

Display images, shapes, particles, text, video, tiles, or even 3D content.

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

class SK3DNode

3D SceneKit content drawn as a flattened sprite.

### Nodes for Environmental Effects

Provide environmental effects to your scene, such as audio, lighting, or areas with specific physics characteristics.

class SKAudioNode

A node that plays audio.

class SKLightNode

A node that lights surrounding nodes.

class SKFieldNode

A node that applies physics effects to nearby nodes.

### Nodes that Modify Drawing

Modify the rendering of child nodes by cropping, applying Core Image filters, or performing 3D transformations.

class SKEffectNode

A node that renders its children into a separate buffer, optionally applying an effect, before drawing the final result.

class SKCropNode

A node that masks pixels drawn by its children so that only some pixels are seen.

class SKTransformNode

A node that allows its children to rotate in 3D.

## See Also

### Essentials

Drawing SpriteKit Content in a View

Display visual content using SpriteKit.

class SKScene

An object that organizes all of the active SpriteKit content.

