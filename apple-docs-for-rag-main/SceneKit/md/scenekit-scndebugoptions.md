

- SceneKit
-  SCNDebugOptions 

Structure

# SCNDebugOptions

Options for drawing overlays with SceneKit content that can aid in debugging, used with the debugOptions property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct SCNDebugOptions
```

## Overview

Debug options are bit mask patterns. To display multiple debugging overlays, combine options using the bitwise OR operator.

## Topics

### Debugging Geometry and Animation

static var showBoundingBoxes: SCNDebugOptions

Display the bounding boxes for any nodes with content.

static var showWireframe: SCNDebugOptions

Display geometries in the scene with wireframe rendering.

static var renderAsWireframe: SCNDebugOptions

Display only wireframe placeholders for geometries in the scene.

static var showSkeletons: SCNDebugOptions

Display visualizations of the skeletal animation parameters for relevant geometries.

static var showCreases: SCNDebugOptions

Display nonsmoothed crease regions for geometries affected by surface subdivision.

static var showConstraints: SCNDebugOptions

Display visualizations of the constraint objects acting on nodes in the scene.

### Debugging Cameras and Lighting

static var showCameras: SCNDebugOptions

Display visualizations for nodes in the scene with attached cameras and their fields of view.

static var showLightInfluences: SCNDebugOptions

Display the locations of each SCNLight object in the scene.

static var showLightExtents: SCNDebugOptions

Display the regions affected by each SCNLight object in the scene.

### Debugging Physics

static var showPhysicsShapes: SCNDebugOptions

Display the physics shapes for any nodes with attached SCNPhysicsBody objects.

static var showPhysicsFields: SCNDebugOptions

Display the regions affected by each SCNPhysicsField object in the scene.

### Initializers

init(rawValue: UInt)

### Type Properties

static let showFeaturePoints: SCNDebugOptions

Display a point cloud showing intermediate results of the scene analysis that ARKit uses to track device position.

static let showWorldOrigin: SCNDebugOptions

Display a coordinate axis visualization indicating the position and orientation of the AR world coordinate system.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Managing Scene Display

var pointOfView: SCNNode?

The node from which the scene’s contents are viewed for rendering.

**Required**

var autoenablesDefaultLighting: Bool

A Boolean value that determines whether SceneKit automatically adds lights to a scene.

**Required**

var isJitteringEnabled: Bool

A Boolean value that determines whether SceneKit applies jittering to reduce aliasing artifacts.

**Required**

var showsStatistics: Bool

A Boolean value that determines whether SceneKit displays rendering performance statistics in an accessory view.

**Required**

var debugOptions: SCNDebugOptions

Options for drawing overlay content in a scene that can aid debugging.

**Required**

var renderingAPI: SCNRenderingAPI

The graphics technology SceneKit uses to render the scene.

**Required**

enum SCNRenderingAPI

Options for choosing the graphics technology for an SCNView object (or other SceneKit renderer) to use for drawing its contents. Used by the renderingAPI property and the preferredRenderingAPI option when initializing an SCNView object.

