

- AppKit
-  NSOpenGLContext Deprecated

Class

# NSOpenGLContext

An object that represents an OpenGL graphics context, into which all OpenGL calls are rendered.

macOS 10.0–10.14Deprecated

``` source
class NSOpenGLContext
```

Deprecated

The OpenGL API is deprecated. Use Metal and MetalKit instead.

## Overview

An OpenGL context is created using an NSOpenGLPixelFormatobject that specifies the context’s buffer types and other attributes. A context can be full-screen, offscreen, or associated with an NSView object. A context draws into its *drawable object*, which is the frame buffer that is the target of OpenGL drawing operations.

Every NSOpenGLContext object wraps a low-level, platform-specific Core OpenGL (CGL) context. Your application can retrieve the CGL context by calling the cglContextObj method. For more information on the underling CGL context, see `CGL`.

## Topics

### Creating Contexts

init?(format: NSOpenGLPixelFormat, share: NSOpenGLContext?)

Returns an OpenGL context object initialized with the specified pixel format information.

init?(cglContextObj: CGLContextObj)

Initializes and returns an OpenGL context object using an existing CGL context.

### Managing the Current Context

class func clearCurrentContext()

Clears the current context.

class var current: NSOpenGLContext?

Returns the current OpenGL graphics context.

func makeCurrentContext()

Sets the context as the current OpenGL context object.

### Managing the Drawable Object

var view: NSView?

Returns the OpenGL context’s view.

func clearDrawable()

Disassociates the OpenGL context from its viewport.

func update()

Updates the OpenGL context’s drawable object.

### Flushing the Drawing Buffer

func flushBuffer()

Copies the back buffer to the front buffer of the OpenGL context.

### Context Parameter Handling

func setValues(UnsafePointer&lt;GLint>, for: NSOpenGLContext.Parameter)

Sets the value of the specified parameter.

func getValues(UnsafeMutablePointer&lt;GLint>, for: NSOpenGLContext.Parameter)

Returns the value of the requested parameter.

### Working with Virtual Screens

var currentVirtualScreen: GLint

Returns the current virtual screen for the OpenGL context.

### Getting the CGL Context Object

var cglContextObj: CGLContextObj?

Returns the low-level, platform-specific Core OpenGL (CGL) context object represented by the receiver.

### Getting the Pixel Format

var pixelFormat: NSOpenGLPixelFormat

The pixel format of the OpenGL context.

### Getting the OpenGL Version

static var openGLVersion: (major: GLint, minor: GLint)

The version of OpenGL.

### Constants

enum Parameter

Constants that specify context parameters.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSLocking
- NSObjectProtocol

## See Also

### Classes

class NSOpenGLView

A view that displays OpenGL content in a view.

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

