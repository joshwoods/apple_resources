

- Quartz
-  QCView Deprecated

Class

# QCView

The `QCView` class is a custom `NSView` class that loads, plays, and controls Quartz Composer compositions. It is an autonomous view that is driven by an internal timer running on the main thread.

macOS 10.4–10.15Deprecated

``` source
@MainActor
class QCView
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Overview

The view can be set to render a composition automatically when it is placed onscreen. The view stops rendering when it is placed offscreen. When not rendering, the view is filled with the current erase color. The rendered composition automatically synchronizes to the vertical retrace of the monitor.

When you archive a `QCView` object, it saves the composition that’s loaded at the time the view is archived.

If you want to perform custom operations while a composition is rendering such as setting input parameters or drawing OpenGL content, you need to subclass `QCView` and implement the render(atTime:arguments:) method.

## Topics

### Performing Custom Operations During Rendering

func render(atTime: TimeInterval, arguments: [AnyHashable : Any]!) -> Bool

Overrides to perform your custom operations prior to or after rendering a frame of a composition.

### Loading a Composition

func loadComposition(fromFile: String!) -> Bool

Loads the composition file located at the specified path.

func load(QCComposition!) -> Bool

Loads a QCComposition object into the view.

func loadedComposition() -> QCComposition!

Returns the composition loaded in the view.

func unloadComposition()

Unloads the composition from the view.

### Managing the Erase Color

func erase()

Clears the view using the current erase color.

func eraseColor() -> NSColor!

Retrieves the current color used to erase the view.

func setEraseColor(NSColor!)

Sets the color used to erase the view.

### Setting and Getting Event Masks

func eventForwardingMask() -> Int

Retrieves the mask used to filter which types of events are forwarded from the view to the composition during rendering.

func setEventForwardingMask(Int)

Sets the mask used to filter which types of events are forwarded from the view to the composition during rendering.

### Setting and Getting the Maximum Frame Rate

func maxRenderingFrameRate() -> Float

Returns the maximum frame rate for rendering.

func setMaxRenderingFrameRate(Float)

Sets the maximum rendering frame rate.

### Managing Rendering

func startRendering() -> Bool

Starts rendering the composition that is in the view.

func isRendering() -> Bool

Checks whether a composition is rendering in the view.

func autostartsRendering() -> Bool

Checks whether the view is set to start rendering automatically.

func setAutostartsRendering(Bool)

Sets whether the composition that is in the view starts rendering automatically when the view is put on the screen.

func stopRendering()

Stops rendering the composition that is in the view.

func pauseRendering()

Pauses rendering in the view.

func isPausedRendering() -> Bool

Returns whether or not the rendering in the view is paused.

func resumeRendering()

Resumes rendering a paused composition.

### Using Interface Builder

func play(Any!)

Plays or pauses a composition in a view.

func start(Any!)

Starts rendering a composition in a view.

func stop(Any!)

Stops rendering a composition in a view.

### Taking Snapshot Images

func snapshotImage() -> NSImage!

Returns an `NSImage` object of the current image in the view.

func createSnapshotImage(ofType: String!) -> Any!

Returns the current image in the view as an image object of the provided image type.

### Working With OpenGL

func openGLContext() -> NSOpenGLContext!

Returns the OpenGL context used by the view.

func openGLPixelFormat() -> NSOpenGLPixelFormat!

Returns the OpenGL pixel format used by the view.

## Relationships

### Inherits From

- NSView

### Conforms To

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
- QCCompositionRenderer
- Sendable

## See Also

### Classes

class QCComposition

The `QCComposition` class represents a Quartz Composer composition that either:

Deprecated

class QCCompositionLayer

A layer that loads, plays, and controls Quartz Composer compositions in a Core Animation layer hierarchy.

Deprecated

class QCCompositionParameterView

A class that allows users to edit the input parameters of a composition in real time. The composition can be rendering in any of the following objects: QCRenderer, QCView, or QCCompositionLayer.

Deprecated

class QCCompositionPickerPanel

The `QCCompositionPickerPanel` class represents a utility window that allows users to browse compositions that are in the Quartz Composer composition repository and, if supported, preview the composition. The `QCCompositionPickerPanel` class cannot be subclassed.

Deprecated

class QCCompositionPickerView

The `QCCompositionPickerView` class allows users to browse compositions that are in the Quartz Composer composition repository, and to preview them. You can set the default input parameters for a composition preview by using the method setDefaultValue:forInputKey:.

Deprecated

class QCCompositionRepository

The `QCCompositionRepository` class represents a system-wide centralized repository of built-in and installed Quartz Composer compositions (`/Library/Compositions` and `~/Library/Compositions`). The `QCCompositionRepository` class cannot be subclassed.

Deprecated

class QCPatchControllerDeprecated

class QCPlugIn

A base class to subclass for writing custom patches.

Deprecated

class QCPlugInViewController

The `QCPlugInViewController` class communicates (through Cocoa bindings) between a custom patch and the view used for the internal settings of the custom patch. Only custom patches that use internal settings exposed to the user need to use the `QCPlugInViewController` class.

Deprecated

class QCRenderer

A base class for low-level rendering.

Deprecated

