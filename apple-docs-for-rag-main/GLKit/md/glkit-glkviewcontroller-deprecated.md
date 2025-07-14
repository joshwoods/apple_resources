

- GLKit
-  GLKViewController Deprecated

Class

# GLKViewController

A view controller that manages an OpenGL ES rendering loop.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
class GLKViewController
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Overview

A GLKViewController object works in conjunction with a GLKView object to display frames of animation in the view, and also provides standard view controller functionality.

To use this class, allocate and initialize a new GLKViewController subclass and set its view property to point to a GLKView object. Then, configure the view controller’s preferredFramesPerSecond property to the desired frame rate your application requires. You can set a delegate or configure other properties on the view controller, such as whether the animation loop is automatically paused or resumed when the application moves into the background.

Note

When you set the view property to point to a GLKView object, if the view does not already have a delegate, then the view controller is automatically set as the view’s delegate.

When active, rendering loop automatically updates the view’s contents each time a new frame must be displayed. Each frame is rendered by the view controller using these steps:

1.  The view controller calls its delegate’s glkViewControllerUpdate(_:) method. Your delegate should update frame data that does not involve rendering the results to the screen.

2.  The view controller calls its view’s display() method. Your view should redraw the frame.

### Subclassing Notes

Your application should subclass GLKViewController and override the viewDidLoad() and viewDidUnload methods. Your `viewDidLoad` method should set up your context and any drawable properties and can perform other resource allocation and initialization. Similarly, your class’s `viewDidUnload` method should delete the drawable object and free any unneeded resources.

As an alternative to implementing a glkViewControllerUpdate(_:) method in a delegate, your subclass can provide an update method instead. The method must have the following signature:

```
- (void)update;
```

## Topics

### Configuring the Frame rate

var preferredFramesPerSecond: Int

The rate you want the view controller to call the view to update the contents of the view.

var framesPerSecond: Int

The actual rate that the view controller attempts to call the view to update its contents.

### Configuring the Delegate

var delegate: (any GLKViewControllerDelegate)?

The view controller’s delegate.

### Controlling Frame Updates

var isPaused: Bool

A Boolean value that indicates whether the rendering loop is paused.

var pauseOnWillResignActive: Bool

A Boolean value that indicates whether the view controller automatically pauses the rendering loop when the application resigns the active state.

var resumeOnDidBecomeActive: Bool

A Boolean value that indicates whether the view controller automatically resumes the rendering loop when the application becomes active.

### Obtaining Information About View Updates

var framesDisplayed: Int

The number of frame updates that have been sent by the view controller since it was created.

var timeSinceFirstResume: TimeInterval

The amount of time that has passed since first time the view controller resumed sending update events.

var timeSinceLastResume: TimeInterval

The amount of time that has passed since the last time the view controller resumed sending update events.

var timeSinceLastUpdate: TimeInterval

The amount of time that has passed since the last time the view controller called the delegate’s glkViewControllerUpdate(_:) method.

var timeSinceLastDraw: TimeInterval

The amount of time that has passed since the last time the view controller called the view’s display() method.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GLKViewDelegate
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### OpenGL ES View Rendering

class GLKView

A default implementation for views that draw their content using OpenGL ES.

Deprecated

protocol GLKViewDelegate

Drawing callback methods for use with a GLKView object.

protocol GLKViewControllerDelegate

Rendering loop callback methods for use with a GLKViewController object.

