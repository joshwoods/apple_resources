

- AppKit
-  NSOpenGLView Deprecated

Class

# NSOpenGLView

A view that displays OpenGL content in a view.

macOS 10.0–10.14Deprecated

``` source
@MainActor
class NSOpenGLView
```

Deprecated

Please use MTKView instead.

## Overview

An NSOpenGLView object maintains an NSOpenGLPixelFormat and NSOpenGLContext object into which OpenGL calls can be rendered. The view provides methods for accessing and managing the NSOpenGLPixelFormat and NSOpenGLContext objects, as well as notifications of visible region changes.

An `NSOpenGLView` object cannot have subviews. You can, however, divide a single `NSOpenGLView` into multiple rendering areas using the `glViewport` function.

When creating an `NSOpenGLView` object in Interface Builder, you use the inspector window to specify the pixel format attributes you want for the view. Only those attributes listed in the Interface Builder inspector are set when the view is instantiated.

Note

In versions of the Xcode Tools that shipped prior to OS X v10.4, the Interface Builder inspector does not list any pixel format attributes for `NSOpenGLView`.

## Topics

### Initializing an NSOpenGLView

init?(frame: NSRect, pixelFormat: NSOpenGLPixelFormat?)

Returns an `NSOpenGLView` object initialized with the specified frame rectangle and pixel format.

### Managing the NSOpenGLPixelFormat

class func defaultPixelFormat() -> NSOpenGLPixelFormat

Returns a default NSOpenGLPixelFormat object.

var pixelFormat: NSOpenGLPixelFormat?

The NSOpenGLPixelFormat object associated with the receiver.

### Managing the NSOpenGLContext

func prepareOpenGL()

Used by subclasses to initialize OpenGL state.

func clearGLContext()

Releases the NSOpenGLContext object associated with the view.

var openGLContext: NSOpenGLContext?

The NSOpenGLContext object associated with the receiver.

### Managing the Visible Region

func reshape()

Called by Cocoa when the view’s visible rectangle or bounds change.

func update()

Called by Cocoa when the view’s window moves or when the view itself moves or is resized.

### Extended Dynamic Range

var wantsExtendedDynamicRangeOpenGLSurface: Bool

Enables extended dynamic range values on the screen.

### Instance Properties

var wantsBestResolutionOpenGLSurface: Bool

A Boolean value indicating whether the view wants an OpenGL backing surface with a resolution greater than 1 pixel per point.

var wantsExtendedDynamicRangeOpenGLSurface: Bool

Enables extended dynamic range values on the screen.

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
- Sendable

## See Also

### Classes

class NSOpenGLContext

An object that represents an OpenGL graphics context, into which all OpenGL calls are rendered.

Deprecated

class NSOpenGLLayer

A subclass of CAOpenGLLayer that is suitable for rendering OpenGL into layers.

Deprecated

class NSOpenGLPixelFormat

An object that specifies the types of buffers and other attributes of the OpenGL context.

Deprecated

class NSDrawer

A user interface element that contains and displays text, scroll, and browser views, in addition to other view subclasses.

Deprecated

class NSForm

An `NSForm` object is a vertical matrix of NSFormCell objects to implement the fields.

Deprecated

class NSFormCell

The `NSFormCell` class is used to implement text entry fields in a form. The left part of an `NSFormCell` object contains a title. The right part contains an editable text entry field.

class NSMenuItemCell

An object that handles the measurement and display of a single menu item in its encompassing frame.

