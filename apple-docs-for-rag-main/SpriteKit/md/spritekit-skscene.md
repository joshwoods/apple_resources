

- SpriteKit
-  SKScene 

Class

# SKScene

An object that organizes all of the active SpriteKit content.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
class SKScene
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKScene
```

## Mentioned in 

Getting Started with Nodes

Subclassing Scenes Versus Assigning a Delegate

Customizing the Behavior of a Node

Controlling User Interaction on Nodes

Creating a Scene from a File

## Overview

An SKScene object represents a scene of content in SpriteKit. A scene is the root node in a tree of SpriteKit nodes (SKNode). These nodes provide content that the scene animates and renders for display. To display a scene, you present it from an SKView, SKRenderer, or WKInterfaceSKScene.

`SKScene` is a subclass of SKEffectNode and enables certain effects to apply to the entire scene. Though applying effects to an entire scene can be an expensive operation, creativity, and ingenuity may help you find some interesting ways to use effects.

## Topics

### Creating a Scene from a File

Creating a Scene from a File

Load a scene that you configure in Xcode’s scene editor.

### Creating a Scene Programmatically

Use code to manually create a scene and configure its properties.

init(size: CGSize)

Initializes a new scene object.

var size: CGSize

The dimensions of the scene, in points.

### Stretching Content to Fit the View

Scaling a Scene’s Content to Fit the View

Configure the scale mode to determine how a scene is sized to fit its view.

var scaleMode: SKSceneScaleMode

A setting that defines how the scene is mapped to the view that presents it.

enum SKSceneScaleMode

The modes that determine how the scene’s area is mapped to the view that presents it.

### Configuring the Viewport

Define which portion of the scene is visible at a given time.

Positioning a Scene’s Origin Within its View

Try the different ways to configure the scene’s origin inside its view.

var camera: SKCameraNode?

The camera node in the scene that determines what part of the scene’s coordinate space is visible in the view.

var anchorPoint: CGPoint

The point in the view’s frame that corresponds to the scene’s origin.

### Responding to Loading and Resizing Events

Override these functions to be notified when a scene is loaded or presented, or changes size.

func sceneDidLoad()

Tells you when the scene is presented.

func didChangeSize(CGSize)

Tells you when the scene’s size has changed.

func willMove(from: SKView)

Tells you when the scene is about to be removed from a view.

func didMove(to: SKView)

Tells you when the scene is presented by a view.

### Responding to Frame-Cycle Events

Callbacks occur every frame, telling you when to perform app logic.

Responding to Frame-Cycle Events

Implement per-frame app logic, such as the scene’s update function that’s called every frame.

func update(TimeInterval)

Tells your app to perform any app-specific logic to update your scene.

func didEvaluateActions()

Tells your app to peform any necessary logic after scene actions are evaluated.

func didSimulatePhysics()

Tells your app to peform any necessary logic after physics simulations are performed.

func didApplyConstraints()

Tells your app to peform any necessary logic after constraints are applied.

func didFinishUpdate()

Tells your app to peform any necessary logic after the scene has finished all of the steps required to process animations.

### Configuring a Delegate

Instead of subclassing a scene to respond to update life-cycle events, assign a delegate to field them.

Subclassing Scenes Versus Assigning a Delegate

Use a scene delegate to share app logic across various scenes.

var delegate: (any SKSceneDelegate)?

A delegate to be called during the animation loop.

protocol SKSceneDelegate

Methods that, when implemented, allow any class to participate in the SpriteKit render loop callbacks.

### Setting the Background Appearance

Adjust content that’s under a scene.

Creating a Scene with a Transparent Background

Set a transparent background color to show the content of the views below.

var view: SKView?

The view that is currently presenting the scene.

var backgroundColor: UIColor

The background color of the scene.

### Configuring Physics Properties

var physicsWorld: SKPhysicsWorld

The physics simulation associated with the scene.

### Adding Positional Audio

Enable positional audio by defining a listener.

Using Audio Nodes with the Scene’s Listener

Add audio to your scene, and optionally give it 2D-positional mixing characteristics.

var listener: SKNode?

A node used to determine the position of the listener for positional audio in the scene.

var audioEngine: AVAudioEngine

The AVFoundation audio engine used to play audio from audio nodes contained in the scene.

### Converting Between Coordinate Systems

func convertPoint(fromView: CGPoint) -> CGPoint

Converts a point from view coordinates to scene coordinates.

func convertPoint(toView: CGPoint) -> CGPoint

Converts a point from scene coordinates to view coordinates.

## Relationships

### Inherits From

- SKEffectNode

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GKSceneRootNodeType
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

### Essentials

Drawing SpriteKit Content in a View

Display visual content using SpriteKit.

Nodes for Scene Building

Define the appearance or layout of scene content.

