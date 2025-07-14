

- GLKit
-  GLKView Deprecated

Class

# GLKView

A default implementation for views that draw their content using OpenGL ES.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
class GLKView
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Overview

The GLKView class simplifies the effort required to create an OpenGL ES application by directly managing a framebuffer object on your behalf; your application simply needs to draw into the framebuffer when the contents need to be updated.

To use this class in your application, create a new GLKView object and provide it an OpenGL ES context. Then, modify the view’s drawableColorFormat, drawableDepthFormat, drawableStencilFormat, and drawableMultisample properties to configure the format of the drawable’s framebuffer object. After this, the view automatically creates or updates the framebuffer object whenever the view must be redrawn. A GLKView object uses the regular view drawing cycle for a UIViewobject, calling its draw(_:) method whenever the contents of the view need to be updated. Before calling its `draw `method, the view makes its EAGLContext object the current OpenGL ES context and binds its framebuffer object to the OpenGL ES context as the target for rendering commands. Your application’s implementation of the `draw` method should call one or more OpenGL ES functions to render an image into the framebuffer object. Then, the view resolves any multisampling that you may have enabled and delivers the finished results.

Important

Your drawing method should only modify the contents of the framebuffer object. Never attempt to read the pixel information from the underlying framebuffer object, modify or dispose of the framebuffer object, or read its other properties by calling OpenGL ES functions. Instead, rely on the properties and methods provided by the GLKView class.

The GLKView class can be used in conjunction with a GLKViewController object to create an animation rendering loop that redraws the contents of the view at a specified frame rate.

### Subclassing Notes

Typically, there is no need to subclass the GLKView class. Instead, provide a delegate object to draw the view’s contents. See GLKViewDelegate.

## Topics

### Initializing the View

init(frame: CGRect, context: EAGLContext)

Initializes a new view.

### Delegate

var delegate: (any GLKViewDelegate)?

The view’s delegate.

### Configuring the Framebuffer Object

var drawableColorFormat: GLKViewDrawableColorFormat

The format of the color renderbuffer.

var drawableDepthFormat: GLKViewDrawableDepthFormat

The format of the depth renderbuffer

var drawableStencilFormat: GLKViewDrawableStencilFormat

The format of the stencil renderbuffer.

var drawableMultisample: GLKViewDrawableMultisample

The format of the multisampling buffer.

### Read-only Framebuffer Properties

var drawableHeight: Int

The height, in pixels, of the underlying framebuffer object.

var drawableWidth: Int

The width, in pixels, of the underlying framebuffer object.

### Drawing Your View’s Contents

var context: EAGLContext

The OpenGL ES context used when drawing the view’s contents.

func bindDrawable()

Binds the underlying framebuffer object to OpenGL ES.

var enableSetNeedsDisplay: Bool

A Boolean value that indicates whether the view responds to messages that invalidate the view’s contents.

func display()

Redraws the view’s contents immediately.

var snapshot: UIImage

Draws the contents of the view and returns them as a new image object.

### Deleting the View’s Underlying Framebuffer Object

func deleteDrawable()

Deletes the drawable object associated with the view.

### Constants

enum GLKViewDrawableColorFormat

The format of the color renderbuffer.

enum GLKViewDrawableDepthFormat

The format of the depth renderbuffer.

enum GLKViewDrawableStencilFormat

The format of the stencil renderbuffer.

enum GLKViewDrawableMultisample

The format of the multisampling buffer.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
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

### OpenGL ES View Rendering

protocol GLKViewDelegate

Drawing callback methods for use with a GLKView object.

class GLKViewController

A view controller that manages an OpenGL ES rendering loop.

Deprecated

protocol GLKViewControllerDelegate

Rendering loop callback methods for use with a GLKViewController object.

