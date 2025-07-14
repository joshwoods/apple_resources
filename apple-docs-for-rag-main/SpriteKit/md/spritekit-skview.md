

- SpriteKit
-  SKView 

Class

# SKView

A view subclass that renders a SpriteKit scene.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
class SKView
```

## Mentioned in 

Choosing a SpriteKit Scene Renderer

Creating a New Node By Rendering To a Texture

## Overview

You present a scene by calling the view’s presentScene(_:) method. When a scene is presented by the view, it alternates between running its simulation (which animates the content) and rendering the content for display. You can pause the scene by setting the view’s isPaused property to true.

## Topics

### Displaying a Scene

Present a scene to display content on the screen.

var scene: SKScene?

The scene currently presented by this view.

func presentScene(SKScene?)

Presents a scene.

func presentScene(SKScene, transition: SKTransition)

Transitions from the current scene to a new scene.

class SKTransition

An object used to perform an animated transition to a new scene.

### Controlling the Timing of a Scene’s Rendering

Control the timing of the view’s screen updates.

var isPaused: Bool

A Boolean value that indicates whether the view’s scene animations are paused.

var preferredFramesPerSecond: Int

The animation frame rate that the view uses to render its scene.

var delegate: (any SKViewDelegate)?

A delegate that allows dynamic control of the view’s render rate.

protocol SKViewDelegate

Methods to take custom control over the view’s render rate.

var frameInterval: Int

The number of frames that must pass before the scene is called to update its contents.

Deprecated

var preferredFrameRate: FloatDeprecated

### Configuring Performance Related Toggles

Control hints that have performance implications which are unique to your app.

var ignoresSiblingOrder: Bool

A Boolean value that indicates whether parent-child and sibling relationships affect the rendering order of nodes in the scene.

var shouldCullNonVisibleNodes: Bool

A Boolean value that indicates whether the view automatically culls non-visible nodes from the rendering tree.

var allowsTransparency: Bool

A Boolean property that indicates whether the view is rendered using transparency.

var isAsynchronous: Bool

A Boolean value that indicates whether the content is rendered asynchronously.

### Enabling Visual Statistics for Debugging

Display metrics in the bottom corner of the view for debugging purposes.

var showsFPS: Bool

A Boolean value that indicates whether the view displays a frame rate indicator.

var showsNodeCount: Bool

A Boolean value that indicates whether the view displays an overlay that shows physics bodies that are visible in the scene.

var showsDrawCount: Bool

A Boolean value that indicates whether the view displays the number of drawing passes it needed to render the view.

var showsQuadCount: Bool

A Boolean value that indicates whether the view displays the number of rectangles used to render the scene.

var showsPhysics: Bool

A Boolean value that indicates whether the view displays physics-related debugging information.

var showsFields: Bool

A Boolean value that indicates whether the view displays information about physics fields in the scene.

### Converting Between View and Scene Coordinates

Convert to or from scene and view coordinates which is a common task for touch or mouse input.

func convert(CGPoint, from: SKScene) -> CGPoint

Converts a point from scene coordinates to view coordinates.

func convert(CGPoint, to: SKScene) -> CGPoint

Converts a point from view coordinates to scene coordinates.

### Snapshotting Nodes to a Texture

Create a texture that is a flattened or cropped portion of the node heirarchy.

func texture(from: SKNode, crop: CGRect) -> SKTexture?

Renders a portion of a node’s contents and returns the rendered image as a texture.

func texture(from: SKNode) -> SKTexture?

Renders the contents of a node tree and returns the rendered image as a texture.

Creating a New Node By Rendering To a Texture

Render a portion of the node tree into a new texture.

### Switching Renderers

Requesting the OpenGL Renderer

Switch to the legacy renderer temporarily for debugging purposes.

### Instance Properties

var disableDepthStencilBuffer: Bool

## Relationships

### Inherits From

- NSView
- UIView

### Conforms To

- CALayerDelegate
- CVarArg
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
- NSSecureCoding
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
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

### Scene Renderers

Choosing a SpriteKit Scene Renderer

Compare the different ways to display a SpriteKit scene.

class SKRenderer

An object that renders a scene into a custom Metal rendering pipeline and drives the scene update cycle.

class WKInterfaceSKScene

A visual WatchKit element that displays a SpriteKit scene.

