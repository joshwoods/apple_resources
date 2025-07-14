

- ARKit
-  ARSKView 

Class

# ARSKView

A view that blends virtual 2D content from SpriteKit into the 3D space of an augmented reality experience.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@MainActor
class ARSKView
```

## Mentioned in 

Providing 2D Virtual Content with SpriteKit

## Overview

Use the ARSKView class to create augmented reality experiences that position 2D elements in 3D space within a device camera view of the real world. When you run the view’s provided ARSession object:

- The view automatically renders the live video feed from the device camera as the scene background.

- When you implement ARSKViewDelegate methods to associate SpriteKit content with real-world positions, the view automatically scales and rotates those SpriteKit nodes so that they appear to track the real world seen by the camera.

## Topics

### First Steps

Providing 2D Virtual Content with SpriteKit

Use SpriteKit to place two-dimensional images in 3D space in your AR experience.

var session: ARSession

The AR session that manages motion tracking and camera image processing for the view’s contents.

### Responding to AR Updates

var delegate: (any ARSKViewDelegate)?

An object you provide to mediate synchronization of the view’s AR scene information with SpriteKit content.

protocol ARSKViewDelegate

Methods you can implement to mediate the automatic synchronization of SpriteKit content with an AR session.

### Finding Real-World Surfaces

func hitTest(CGPoint, types: ARHitTestResult.ResultType) -> [ARHitTestResult]

Searches for real-world objects or AR anchors in the captured camera image corresponding to a point in the SpriteKit view.

Deprecated

### Mapping Content to Real-World Positions

func anchor(for: SKNode) -> ARAnchor?

Returns the AR anchor associated with the specified SpriteKit node, if any.

func node(for: ARAnchor) -> SKNode?

Returns the SpriteKit node associated with the specified AR anchor, if any.

## Relationships

### Inherits From

- SKView

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

class ARSCNView

A view that blends virtual 3D content from SceneKit into your augmented reality experience.

class ARCoachingOverlayView

A view that displays standardized onboarding instructions to direct users toward a specific goal.

