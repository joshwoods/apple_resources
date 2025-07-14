

- AppKit
-  NSOpenGLLayer Deprecated

Class

# NSOpenGLLayer

A subclass of CAOpenGLLayer that is suitable for rendering OpenGL into layers.

macOS 10.6–10.14Deprecated

``` source
class NSOpenGLLayer
```

Deprecated

The OpenGL API is deprecated. Use Metal and MetalKit instead.

## Overview

Unlike CAOpenGLLayer, NSOpenGLLayer uses AppKit types.

## Topics

### Drawing the Content

func canDraw(in: NSOpenGLContext, pixelFormat: NSOpenGLPixelFormat, forLayerTime: CFTimeInterval, displayTime: UnsafePointer&lt;CVTimeStamp>) -> Bool

Invoked to ask the layer whether it can (or should) draw.

func draw(in: NSOpenGLContext, pixelFormat: NSOpenGLPixelFormat, forLayerTime: CFTimeInterval, displayTime: UnsafePointer&lt;CVTimeStamp>)

Draws the OpenGL content for the specified time.

### Managing the Pixel Format

var openGLPixelFormat: NSOpenGLPixelFormat?

Provides access to the layer’s associated OpenGL pixel format.

func openGLPixelFormat(forDisplayMask: UInt32) -> NSOpenGLPixelFormat

Returns the OpenGL pixel format suitable for the specified displays.

### Managing the Rendering Context

var openGLContext: NSOpenGLContext?

The layer’s OpenGL context.

func openGLContext(for: NSOpenGLPixelFormat) -> NSOpenGLContext

Returns the OpenGL context to use for the requested pixel format.

### Accessing the Associated View

var view: NSView?

Returns the view associated with the layer.

## Relationships

### Inherits From

- CAOpenGLLayer

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Classes

class NSOpenGLView

A view that displays OpenGL content in a view.

Deprecated

class NSOpenGLContext

An object that represents an OpenGL graphics context, into which all OpenGL calls are rendered.

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

