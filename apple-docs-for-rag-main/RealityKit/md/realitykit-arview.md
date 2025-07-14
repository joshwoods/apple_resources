

- RealityKit
-  ARView 

Class

# ARView

A view that enables you to display an AR experience with RealityKit.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
@MainActor @objc @preconcurrency
class ARView
```

## Mentioned in 

Handling different-sized objects in physics simulations

Implementing postprocess effects using Metal compute functions

Using Metal performance shaders to create custom postprocess effects

Loading Reality Composer files using generated code

Taking Control of Scene Anchoring

## Overview

Use an ARView instance to display rendered 3D graphics to the user. You typically add a single view to your app’s storyboard, and then provide an outlet for that view in your code. Alternatively, you can create and add a view to your view hierarchy programmatically at runtime, as you would any other view.

A view has a single Scene instance that you access through the read-only scene property. To the view’s Scene instance you add one or more AnchorEntity instances that tell the view’s AR session how to tether content to something in the real world. To each anchor, you attach a hierarchy of other Entity instances that make up the content of the scene.

Additionally, you can use the view to:

- Configure render options, environmental characteristics, and the camera mode.

- Handle platform-appropriate user interaction in the form of mouse, keyboard, or gesture input.

- Find entities at a given point in the view.

- Access statistics and visualizations that help you debug your app.

Note that with ARView, a ModelEntity casts a grounding shadow on a physical surface by default. RealityView does not have this default behavior.

## Topics

### Creating a view

init(frame: CGRect)

Creates an AR view with the specified dimensions.

init(frame: CGRect, cameraMode: ARView.CameraMode, automaticallyConfigureSession: Bool)

Creates an AR view with the specified dimensions, camera mode, and session configuration state.

init?(coder: NSCoder)

Creates an AR view initialized from data in a given decoder.

convenience init(frame: CGRect, cameraMode: ARView.CameraMode)

Creates an AR view with the specified dimensions and camera mode.

Deprecated

### Working with the scene

var scene: Scene

The scene that the view renders and simulates.

### Configuring the AR session

var session: ARSession

The AR session that supports the view’s rendering.

var automaticallyConfigureSession: Bool

An indication of whether to use an automatically configured AR session.

var renderOptions: ARView.RenderOptions

The render options that configure the view’s AR session.

var renderCallbacks: ARView.RenderCallbacks

A container that holds the view’s render callbacks.

### Providing environmental context

var environment: ARView.Environment

The view’s background, lighting, and acoustic properties.

var physicsOrigin: Entity?

The entity that defines the origin of the scene’s physics simulation.

var audioListener: Entity?

The entity that defines the listener position and orientation for spatial audio.

### Managing the camera

var cameraMode: ARView.CameraMode

A setting that chooses between the AR session’s camera and a virtual one.

var cameraTransform: Transform

The transform of the currently active camera.

### Finding entities at a point in the view

func entity(at: CGPoint) -> Entity?

Finds the entity in the AR scene closest to the specified point.

func entities(at: CGPoint) -> [Entity]

Finds the collection of entities at the specified point in the scene.

func hitTest(CGPoint, query: CollisionCastQueryType, mask: CollisionGroup) -> [CollisionCastHit]

Searches for objects corresponding to a point in the view based on a query and a collision mask.

func hitTest(CGPoint, types: ARHitTestResult.ResultType) -> [ARHitTestResult]

Searches for objects corresponding to a point in the view based on a set of result types.

func makeRaycastQuery(from: CGPoint, allowing: ARRaycastQuery.Target, alignment: ARRaycastQuery.TargetAlignment) -> ARRaycastQuery?

Creates a ray-cast query originating from a point in the view, centered on the camera’s field of view.

func raycast(from: CGPoint, allowing: ARRaycastQuery.Target, alignment: ARRaycastQuery.TargetAlignment) -> [ARRaycastResult]

Performs a ray cast, where a ray is cast into the scene from the center of the camera through a point in the view, and the results are immediately returned.

func trackedRaycast(from: CGPoint, allowing: ARRaycastQuery.Target, alignment: ARRaycastQuery.TargetAlignment, updateHandler: ([ARRaycastResult]) -> Void) -> ARTrackedRaycast?

Performs a tracked ray cast, where a ray is cast into the scene from the center of the camera through a point in the view.

### Adding gesture recognizers to entities

func installGestures(ARView.EntityGestures, for: any HasCollision) -> [any EntityGestureRecognizer]

Installs standard gestures onto the given entity, configured to be recognized simultaneously.

func gestureRecognizer(UIGestureRecognizer, shouldRecognizeSimultaneouslyWith: UIGestureRecognizer) -> Bool

### Mapping between coordinate spaces

func project(SIMD3&lt;Float>) -> CGPoint?

Projects a point from the 3D world coordinate system of the scene to the 2D pixel coordinate system of the view.

func unproject(CGPoint, ontoPlane: float4x4, relativeToCamera: Bool) -> SIMD3&lt;Float>?

Unproject a 2D point from the view onto a plane in 3D world coordinates.

func unproject(CGPoint, ontoPlane: float4x4) -> SIMD3&lt;Float>?

Maps a 2D point from the view’s coordinate system onto the given plane in 3D space.

func unproject(CGPoint, viewport: CGRect) -> SIMD3&lt;Float>?

Maps a 2D point from the pixel coordinate system of a viewport into a 3D coordinate space. The point lies on this view’s near clipping plane.

func ray(through: CGPoint) -> (origin: SIMD3&lt;Float>, direction: SIMD3&lt;Float>)?

Determines the position and direction of a ray through the given point in the 2D space of the view.

### Handling touch input

func touchesBegan(Set&lt;UITouch>, with: UIEvent?)

Tells the view that one or more new touches occurred.

func touchesMoved(Set&lt;UITouch>, with: UIEvent?)

Tells the view when one or more touches associated with an event changed.

func touchesEnded(Set&lt;UITouch>, with: UIEvent?)

Tells the view when one or more fingers are raised from the view.

func touchesCancelled(Set&lt;UITouch>, with: UIEvent?)

Tells the view when a system event (such as a system alert) cancels a touch sequence.

### Handling keyboard input

var acceptsFirstResponder: Bool

A Boolean value that indicates whether the view accepts first responder status.

func keyDown(with: NSEvent)

Informs the view that the user has pressed a key.

func keyUp(with: NSEvent)

Informs the view that the user has released a key.

### Handling mouse input

func mouseDown(with: NSEvent)

Informs the view that the user has pressed the left mouse button.

func mouseDragged(with: NSEvent)

Informs the view that the user has moved the mouse with the left button pressed.

func mouseUp(with: NSEvent)

Informs the view that the user has released the left mouse button.

func mouseMoved(with: NSEvent)

Informs the view that the mouse has moved.

func rightMouseDown(with: NSEvent)

Informs the view that the user has pressed the right mouse button.

func rightMouseDragged(with: NSEvent)

Informs the view that the user has moved the mouse with the right button pressed.

func rightMouseUp(with: NSEvent)

Informs the view that the user has released the right mouse button.

func otherMouseDown(with: NSEvent)

Informs the view that the user has pressed a mouse button other than the left or right one.

func otherMouseDragged(with: NSEvent)

Informs the view that the user has moved the mouse with a button other than the left or right button pressed.

func otherMouseUp(with: NSEvent)

Informs the view that the user has released a mouse button other than the left or right button.

func scrollWheel(with: NSEvent)

Informs the view that the mouse’s scroll wheel has moved.

### Managing the view

var frame: NSRect

The frame rectangle, which describes the view’s location and size in the coordinate system of the view’s superview.

var contentScaleFactor: CGFloat

The scale factor of the content in the view.

func didMoveToSuperview()

Tells the view that its superview changed.

func didMoveToWindow()

Tells the view that its window property is set to a new value.

func layoutSubviews()

Lays out subviews.

func layout()

class var layerClass: AnyClass

The class used to create the layer for view instances.

func makeBackingLayer() -> CALayer

Creates the view’s backing layer.

func viewDidChangeBackingProperties()

Tells the view when its backing store properties change.

func viewDidMoveToSuperview()

Tells the view that it has a new superview or that the view’s superview has been removed.

### Taking a snapshot

func snapshot(saveToHDR: Bool, completion: (ARView.Image?) -> Void)

Takes a screenshot.

func snapshot(saveToHDR: Bool, completion: (ARView.Image?) -> Void)

Takes a screenshot.

typealias Image

### Debugging the session

Improving the Performance of a RealityKit App

Measure CPU and GPU utilization to find ways to improve your app’s performance.

var debugOptions: ARView.DebugOptions

The current debugging options.

### Structures

struct DebugOptions

Options for drawing overlay content in a scene that can aid in debugging.

struct EntityGestures

The set of possible entity gesture recognizers.

struct Environment

A description of background, lighting, and acoustic properties for a view’s content.

struct PostProcessContext

An object the framework uses to pass data to a postprocess callback.

struct RenderCallbacks

A container that holds the view’s render callbacks.

struct RenderOptions

The available rendering options that you use to selectively disable certain rendering effects.

### Instance Methods

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UITouch) -> Bool

### Enumerations

enum CameraMode

The available camera modes.

### Default Implementations

ARSessionProviding Implementations

## Relationships

### Inherits From

- NSView
- UIView

### Conforms To

- ARSessionProviding
- CALayerDelegate
- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIGestureRecognizerDelegate
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### UIKit and AppKit presentation

struct DebugOptions

Options for drawing overlay content in a scene that can aid in debugging.

typealias ARViewBase

The platform-specific base class for the view into which RealityKit renders content.

