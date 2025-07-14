

- ARKit
-  ARSCNView 

Class

# ARSCNView

A view that blends virtual 3D content from SceneKit into your augmented reality experience.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@MainActor
class ARSCNView
```

## Overview

The ARSCNView class provides the easiest way to create augmented reality experiences that blend virtual 3D content with a device camera view of the real world. When you run the view’s provided ARSession object:

- The view automatically renders the live video feed from the device camera as the scene background.

- The world coordinate system of the view’s SceneKit scene directly responds to the AR world coordinate system established by the session configuration.

- The view automatically moves its SceneKit camera to match the real-world movement of the device.

ARKit automatically matches SceneKit’s coordinate space to the real world, so after you place your app’s virtual content, it maintains the illusion of resting in the real-world as the user moves the device. See Providing 3D Virtual Content with SceneKit.

You don’t necessarily need to use the ARAnchor class to track positions of objects you add to the scene, but by implementing ARSCNViewDelegate methods, you can add SceneKit content to any anchors that are automatically detected by ARKit.

Because ARKit requires Metal, use only Metal features of SceneKit. For example:

- This class supports only SCNProgram instances with Metal Shading Language code.

- If you set the preferredRenderingAPI property to SCNRenderingAPI.openGLES2, the framework reverts the value to SCNRenderingAPI.metal.

## Topics

### Essentials

Providing 3D Virtual Content with SceneKit

Use SceneKit to add realistic three-dimensional objects to your AR experience.

var session: ARSession

The AR session that manages motion tracking and camera image processing for the view’s contents.

var scene: SCNScene

The SceneKit scene to be displayed in the view.

### Responding to AR Updates

var delegate: (any ARSCNViewDelegate)?

An object you provide to mediate synchronization of the view’s AR scene information with SceneKit content.

protocol ARSCNViewDelegate

Methods you can implement to mediate the automatic synchronization of SceneKit content with an AR session.

### Finding Real-World Surfaces

func hitTest(CGPoint, types: ARHitTestResult.ResultType) -> [ARHitTestResult]

Searches for real-world objects or AR anchors in the captured camera image corresponding to a point in the SceneKit view.

Deprecated

func raycastQuery(from: CGPoint, allowing: ARRaycastQuery.Target, alignment: ARRaycastQuery.TargetAlignment) -> ARRaycastQuery?

Creates a raycast query that originates from a point on the view, aligned with the center of the camera’s field of view.

### Mapping Content to Real-World Positions

func anchor(for: SCNNode) -> ARAnchor?

Returns the AR anchor associated with the specified SceneKit node, if any.

func node(for: ARAnchor) -> SCNNode?

Returns the SceneKit node associated with the specified AR anchor, if any.

func unprojectPoint(CGPoint, ontoPlane: simd_float4x4) -> simd_float3?

Returns the projection of a point from 2D view onto a plane in the 3D world space detected by ARKit.

### Managing Lighting

var automaticallyUpdatesLighting: Bool

A Boolean value that specifies whether ARKit creates and updates SceneKit lights in the view’s scene.

### Debugging AR Display

typealias ARSCNDebugOptions

Options for drawing overlay content to aid debugging of AR tracking in a SceneKit view.

### Managing Rendering Effects

var rendersMotionBlur: Bool

Determines whether the view renders motion blur.

var rendersCameraGrain: Bool

A flag that determines whether SceneKit applies image noise characteristics to your app’s virtual content.

## Relationships

### Inherits From

- SCNView

### Conforms To

- ARSessionProviding
- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- SCNSceneRenderer
- SCNTechniqueSupport
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Views

@MainActor @objc @preconcurrency class ARView

A view that enables you to display an AR experience with RealityKit.

class ARSKView

A view that blends virtual 2D content from SpriteKit into the 3D space of an augmented reality experience.

class ARCoachingOverlayView

A view that displays standardized onboarding instructions to direct users toward a specific goal.

