

- SceneKit
-  SCNView 

Class

# SCNView

A view for displaying 3D SceneKit content.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
class SCNView
```

## Overview

In macOS, SCNView is a subclass of NSView. In iOS and tvOS, SCNView is a subclass of UIView. As part of either operating system’s view hierarchy, an SCNView object provides a place for SceneKit content in your app’s user interface. You can create a SceneKit view by using its init(frame:options:) method or by adding it to a nib file or storyboard. To provide content for a SceneKit view, assign an SCNScene object to its scene property.

For additional important methods and properties for working with SceneKit views, see the SCNSceneRenderer protocol. (You can also render SceneKit content into an arbitrary Metal command queue or OpenGL context using the SCNRenderer class, or into a Core Animation layer on macOS using the SCNLayer class. The SCNSceneRenderer protocol defines functionality common to all three SceneKit rendering classes.)

## Topics

### Initializing a SceneKit View

init(frame: CGRect, options: [String : Any]?)

Initializes and returns a newly allocated SceneKit view object with the specified frame rectangle and options.

struct Option

Dictionary keys specifying initialization options, used when initializing a SceneKit view.

### Specifying a Scene

var scene: SCNScene?

The scene to be displayed in the view.

### Configuring a View

var backgroundColor: NSColor

The background color of the view.

var preferredFramesPerSecond: Int

The animation frame rate that the view uses to render its scene.

var rendersContinuously: Bool

A Boolean value that determines whether the view always renders at its preferred frame rate or only when its visible content changes.

var antialiasingMode: SCNAntialiasingMode

The antialiasing mode used for rendering the view’s scene.

enum SCNAntialiasingMode

Modes for antialiased rendering of the view’s scene, used by the SCNView property.

### Managing Camera Controls

var allowsCameraControl: Bool

A Boolean value that determines whether the user can manipulate the current point of view that is used to render the scene.

var cameraControlConfiguration: any SCNCameraControlConfiguration

The current configuration for the camera controller’s event-handling behavior.

protocol SCNCameraControlConfiguration

Properties affecting the behavior of a camera controller.

var defaultCameraController: SCNCameraController

class SCNCameraController

### Playing Action and Animation in a View’s Scene

func pause(Any?)

Pauses playback of the view’s scene.

func play(Any?)

Resumes playback of the view’s scene.

func stop(Any?)

Stops playback of the view’s scene and resets the scene time to its start time.

### Capturing a View Snapshot

func snapshot() -> UIImage

Renders the view’s scene into a new image object.

### Working with a View’s OpenGL ES Context

var eaglContext: EAGLContext?

The OpenGL ES context that the view uses to render its contents.

Deprecated

### Working with a View’s OpenGL Context

var openGLContext: NSOpenGLContext?

The OpenGL context that the view uses to render its contents.

Deprecated

var pixelFormat: NSOpenGLPixelFormat?

The view’s OpenGL pixel format.

Deprecated

### Instance Properties

var drawableResizesAsynchronously: Bool

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
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- SCNSceneRenderer
- SCNTechniqueSupport
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

### Essentials

class SCNScene

A container for the node hierarchy and global properties that together form a displayable 3D scene.

