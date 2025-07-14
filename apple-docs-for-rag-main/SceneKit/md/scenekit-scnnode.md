

- SceneKit
-  SCNNode 

Class

# SCNNode

A structural element of a scene graph, representing a position and transform in a 3D coordinate space, to which you can attach geometry, lights, cameras, or other displayable content.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNNode
```

## Mentioned in 

Animating SceneKit Content

## Overview

An SCNNode object by itself has no visible content when the scene containing it is rendered—it represents only a coordinate space transform (position, orientation, and scale) relative to its parent node. To construct a scene, you use a hierarchy of nodes to create its structure, then add lights, cameras, and geometry to nodes to create visible content.

### Nodes Determine the Structure of a Scene

The hierarchy of nodes, or **scene graph**, in a scene defines both the organization of its contents and your ability to present and manipulate those contents using SceneKit. You may create a node hierarchy programmatically using SceneKit, load one from a file created using 3D authoring tools, or combine the two approaches. SceneKit provides many utilities for organizing and searching the scene graph—for details, see the methods in Managing the Node Hierarchy and Searching the Node Hierarchy.

The rootNode object in a scene defines the coordinate system of the world rendered by SceneKit. Each child node you add to this root node creates its own coordinate system, which is in turn inherited by its own children. You determine the transformation between coordinate systems using the node’s position, rotation, and scale properties properties (or directly using its transform property).

You use a hierarchy of nodes and transformations to model the contents of your scene in a way that suits the needs of your app. For example, if your app presents an animated view of a solar system, you can construct a node hierarchy that models celestial bodies relative to one another: Each planet can be a node, with its orbit and its current position in that orbit defined in the coordinate system of the sun. A planet node defines its own coordinate space, useful both for specifying the planet’s rotation and the orbits of its moons (each of which is a child node of its planet). With this scene hierarchy, you can easily add realistic animation to the scene—animating both the revolution of a moon around its planet and the planet around the sun will combine the animations so that the moon follows the planet.

### A Node’s Attachments Define Visual Content and Behavior

The node hierarchy determines the spatial and logical structure of a scene, but not its visible contents. You add 2D and 3D objects to a scene by attaching SCNGeometry objects to nodes. (Geometries, in turn, have attached SCNMaterial objects that determine their appearance.) To shade the geometries in a scene with light and shadow effects, add nodes with attached SCNLight objects. To control the viewpoint from which the scene appears when rendered, add nodes with attached SCNCamera objects.

To add physics-based behaviors and special effects to SceneKit content, use other types of node attachments. For example, an SCNPhysicsBody object defines a node’s characteristics for physics simulation, and an SCNPhysicsField object applies forces to physics bodies in an area around the node. An SCNParticleSystem object attached to a node renders particle effects such as fire, rain, or falling leaves in the space defined by a node.

To improve performance, SceneKit can share attachments between multiple nodes. For example, in a racing game that includes many identical cars, the scene graph would contain many nodes—one to position and animate each car—but all car nodes would reference the same geometry object.

## Topics

### Creating a Node

init(geometry: SCNGeometry?)

Creates and returns a node object with the specified geometry attached.

### Managing the Node’s Transform

var simdTransform: simd_float4x4

The transform applied to the node relative to its parent. Animatable.

var simdPosition: simd_float3

The translation applied to the node. Animatable.

var simdRotation: simd_float4

The node’s orientation, expressed as a rotation angle about an axis. Animatable.

var simdEulerAngles: simd_float3

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

var simdOrientation: simd_quatf

The node’s orientation, expressed as a quaternion. Animatable.

var simdScale: simd_float3

The scale factor applied to the node. Animatable.

var simdPivot: simd_float4x4

The pivot point for the node’s position, rotation, and scale. Animatable.

### Managing Node Content

var name: String?

A name associated with the node.

var light: SCNLight?

The light attached to the node.

var camera: SCNCamera?

The camera attached to the node.

var geometry: SCNGeometry?

The geometry attached to the node.

var morpher: SCNMorpher?

The morpher object responsible for blending the node’s geometry.

var skinner: SCNSkinner?

The skinner object responsible for skeletal animations of node’s contents.

var categoryBitMask: Int

A mask that defines which categories the node belongs to.

protocol SCNBoundingVolume

Methods common to the SCNNode and SCNGeometry classes for measuring location and size.

### Constraining Node Behavior

var constraints: [SCNConstraint]?

A list of constraints affecting the node’s transformation.

### Working with Node Animation

var presentation: SCNNode

A node object representing the state of the node as it currently appears onscreen.

var isPaused: Bool

A Boolean value that determines whether to run actions and animations attached to the node and its child nodes.

### Modifying the Node Visibility

var isHidden: Bool

A Boolean value that determines the visibility of the node’s contents. Animatable.

var opacity: CGFloat

The opacity value of the node. Animatable.

var renderingOrder: Int

The order the node’s content is drawn in relative to that of other nodes.

var castsShadow: Bool

A Boolean value that determines whether SceneKit renders the node’s contents into shadow maps.

var movabilityHint: SCNMovabilityHint

A value that indicates how SceneKit should handle the node when rendering movement-related effects.

enum SCNMovabilityHint

Values that inform SceneKit’s rendering for movement-related effects, used by the movabilityHint property.

### Managing the Node Hierarchy

var parent: SCNNode?

The node’s parent in the scene graph hierarchy.

var childNodes: [SCNNode]

An array of the node’s children in the scene graph hierarchy.

func addChildNode(SCNNode)

Adds a node to the node’s array of children.

func insertChildNode(SCNNode, at: Int)

Adds a node to the node’s array of children at a specified index.

func removeFromParentNode()

Removes the node from its parent’s array of child nodes.

func replaceChildNode(SCNNode, with: SCNNode)

Removes a child from the node’s array of children and inserts another node in its place.

### Searching the Node Hierarchy

func childNodes(passingTest: (SCNNode, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> [SCNNode]

Returns all nodes in the node’s child node subtree that satisfy the test applied by a block.

func childNode(withName: String, recursively: Bool) -> SCNNode?

Returns the first node in the node’s child node subtree with the specified name.

func enumerateChildNodes((SCNNode, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified block for each of the node’s child and descendant nodes.

func enumerateHierarchy((SCNNode, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified block for each of the node’s child and descendant nodes, as well as for the node itself.

### Customizing Node Rendering

var filters: [CIFilter]?

An array of Core Image filters to be applied to the rendered contents of the node.

var rendererDelegate: (any SCNNodeRendererDelegate)?

An object responsible for rendering custom contents for the node using Metal or OpenGL.

### Adding Physics to a Node

var physicsBody: SCNPhysicsBody?

The physics body associated with the node.

var physicsField: SCNPhysicsField?

The physics field associated with the node.

### Working with Particle Systems

func addParticleSystem(SCNParticleSystem)

Attaches a particle system to the node.

var particleSystems: [SCNParticleSystem]?

The particle systems attached to the node.

func removeParticleSystem(SCNParticleSystem)

Removes a particle system attached to the node.

func removeAllParticleSystems()

Removes any particle systems directly attached to the node.

### Working with Positional Audio

func addAudioPlayer(SCNAudioPlayer)

Adds the specified auto player to the node and begins playback.

var audioPlayers: [SCNAudioPlayer]

The audio players currently attached to the node.

func removeAudioPlayer(SCNAudioPlayer)

Removes the specified audio player from the node, stopping playback.

func removeAllAudioPlayers()

Removes all audio players attached to the node, stopping playback.

### Copying a Node

func clone() -> Self

Creates a copy of the node and its children.

func flattenedClone() -> Self

Creates an optimized copy of the node and its children.

### Hit-Testing

func hitTestWithSegment(from: SCNVector3, to: SCNVector3, options: [String : Any]?) -> [SCNHitTestResult]

Searches the node’s child node subtree for objects intersecting a line segment between two specified points.

struct SCNHitTestOption

Options affecting the behavior of SceneKit hit-testing methods.

### Performing Node-Relative Operations

func simdRotate(by: simd_quatf, aroundTarget: simd_float3)

Changes the node’s position and orientation, relative to its current transform, through a rotation around the specified point in scene space.

func simdLocalTranslate(by: simd_float3)

Changes the node’s position relative to its current position.

func simdLocalRotate(by: simd_quatf)

Changes the node’s orientation relative to its current orientation.

func simdLook(at: simd_float3)

Changes the node’s orientation so that its local forward vector points toward the specified location.

func simdLook(at: simd_float3, up: simd_float3, localFront: simd_float3)

Changes the node’s orientation so that the specified forward vector points toward the specified location.

### Calculating Node-Relative Transforms

class var simdLocalRight: simd_float3

The direction SceneKit treats as “right” in local space for all nodes.

class var simdLocalUp: simd_float3

The direction SceneKit treats as “up” in local space for all nodes.

class var simdLocalFront: simd_float3

The unit vector SceneKit treats as “forward” in local space for all nodes.

var simdWorldRight: simd_float3

The “right” (+X) direction vector relative to the node, expressed in world space.

var simdWorldUp: simd_float3

The “up” (+Y) direction vector relative to the node, expressed in world space.

var simdWorldFront: simd_float3

The “forward” (-Z) direction vector relative to the node, expressed in world space.

### Managing Transforms in World Space

var simdWorldTransform: simd_float4x4

The world transform applied to the node.

var simdWorldOrientation: simd_quatf

The node’s orientation relative to the scene’s world coordinate space.

var simdWorldPosition: simd_float3

The node’s position relative to the scene’s world coordinate space.

### Converting Between Coordinate Spaces

func simdConvertPosition(simd_float3, from: SCNNode?) -> simd_float3

Converts a position to the node’s local coordinate space from that of another node.

func simdConvertPosition(simd_float3, to: SCNNode?) -> simd_float3

Converts a position from the node’s local coordinate space to that of another node.

func simdConvertTransform(simd_float4x4, from: SCNNode?) -> simd_float4x4

Converts a transform to the node’s local coordinate space from that of another node.

func simdConvertTransform(simd_float4x4, to: SCNNode?) -> simd_float4x4

Converts a transform from the node’s local coordinate space to that of another node.

func simdConvertVector(simd_float3, from: SCNNode?) -> simd_float3

Converts a direction vector to the node’s local coordinate space from that of another node.

func simdConvertVector(simd_float3, to: SCNNode?) -> simd_float3

Converts a direction vector from the node’s local coordinate space to that of another node.

### Handling UI Focus

var focusBehavior: SCNNodeFocusBehavior

The focus behavior for a node.

enum SCNNodeFocusBehavior

Options for the focusable states of a SceneKit node.

### Working with GameplayKit

var entity: GKEntity?

The GameplayKit entity this node represents.

### Managing the Node’s Transform (SceneKit Types)

var transform: SCNMatrix4

The transform applied to the node relative to its parent. Animatable.

var position: SCNVector3

The translation applied to the node. Animatable.

var rotation: SCNVector4

The node’s orientation, expressed as a rotation angle about an axis. Animatable.

var eulerAngles: SCNVector3

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

var orientation: SCNQuaternion

The node’s orientation, expressed as a quaternion. Animatable.

var scale: SCNVector3

The scale factor applied to the node. Animatable.

var pivot: SCNMatrix4

The pivot point for the node’s position, rotation, and scale. Animatable.

### Performing Node-Relative Operations (SceneKit Types)

func rotate(by: SCNQuaternion, aroundTarget: SCNVector3)

Changes the node’s position and orientation, relative to its current transform, through a rotation around the specified point in scene space.

func localTranslate(by: SCNVector3)

Changes the node’s position relative to its current position.

func localRotate(by: SCNQuaternion)

Changes the node’s orientation relative to its current orientation.

func look(at: SCNVector3)

Changes the node’s orientation so that its local forward vector points toward the specified location.

func look(at: SCNVector3, up: SCNVector3, localFront: SCNVector3)

Changes the node’s orientation so that the specified forward vector points toward the specified location.

### Calculating Node-Relative Transforms (SceneKit Types)

class var localRight: SCNVector3

The direction SceneKit treats as “right” in local space for all nodes.

class var localUp: SCNVector3

The direction SceneKit treats as “up” in local space for all nodes.

class var localFront: SCNVector3

The unit vector SceneKit treats as “forward” in local space for all nodes.

var worldRight: SCNVector3

The “right” (+X) direction vector relative to the node, expressed in world space.

var worldUp: SCNVector3

The “up” (+Y) direction vector relative to the node, expressed in world space.

var worldFront: SCNVector3

The “forward” (-Z) direction vector relative to the node, expressed in world space.

### Managing Transforms in World Space (SceneKit Types)

var worldTransform: SCNMatrix4

The world transform applied to the node.

func setWorldTransform(SCNMatrix4)

Sets the world transform applied to the node.

var worldOrientation: SCNQuaternion

The node’s orientation relative to the scene’s world coordinate space.

var worldPosition: SCNVector3

The node’s position relative to the scene’s world coordinate space.

### Converting Between Coordinate Spaces (SceneKit Types)

func convertPosition(SCNVector3, from: SCNNode?) -> SCNVector3

Converts a position to the node’s local coordinate space from that of another node.

func convertPosition(SCNVector3, to: SCNNode?) -> SCNVector3

Converts a position from the node’s local coordinate space to that of another node.

func convertTransform(SCNMatrix4, from: SCNNode?) -> SCNMatrix4

Converts a transform to the node’s local coordinate space from that of another node.

func convertTransform(SCNMatrix4, to: SCNNode?) -> SCNMatrix4

Converts a transform from the node’s local coordinate space to that of another node.

func convertVector(SCNVector3, from: SCNNode?) -> SCNVector3

Converts a direction vector to the node’s local coordinate space from that of another node.

func convertVector(SCNVector3, to: SCNNode?) -> SCNVector3

Converts a direction vector from the node’s local coordinate space to that of another node.

## Relationships

### Inherits From

- NSObject

### Inherited By

- SCNReferenceNode

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
- SCNActionable
- SCNAnimatable
- SCNBoundingVolume
- UIFocusEnvironment
- UIFocusItem

## See Also

### Scene Structure

Organizing a Scene with Nodes

Use nodes to define the structure of a scene.

class SCNReferenceNode

A scene graph node that serves as a placeholder for content to be loaded from a separate scene file.

