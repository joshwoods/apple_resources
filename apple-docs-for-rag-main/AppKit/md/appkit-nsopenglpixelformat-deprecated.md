

- AppKit
-  NSOpenGLPixelFormat Deprecated

Class

# NSOpenGLPixelFormat

An object that specifies the types of buffers and other attributes of the OpenGL context.

macOS 10.0–10.14Deprecated

``` source
class NSOpenGLPixelFormat
```

Deprecated

The OpenGL API is deprecated. Use Metal and MetalKit instead.

## Overview

To render with OpenGL into an NSOpenGLContext, you must specify the context’s pixel format. The NSOpenGLPixelFormat class is similar to the AGLPixelFormat type.

Every NSOpenGLPixelFormat object wraps a low-level, platform-specific Core OpenGL (CGL) pixel format object. Your application can retrieve the CGL pixel format object by calling the cglPixelFormatObj method. For more information on the underling CGL pixel format object, see `CGL`.

## Topics

### Creating an OpenGL Pixel Format

init?(cglPixelFormatObj: CGLPixelFormatObj)

Returns an OpenGL pixel format object initialized with using an existing CGL pixel format object.

convenience init?(attributes: UnsafePointer&lt;NSOpenGLPixelFormatAttribute>)

Returns an OpenGL pixel format object initialized with specified pixel format attributes.

### Managing the Pixel Format

var cglPixelFormatObj: CGLPixelFormatObj?

The low-level, platform-specific Core OpenGL (CGL) pixel format object represented by the receiver.

func getValues(UnsafeMutablePointer&lt;GLint>, forAttribute: NSOpenGLPixelFormatAttribute, forVirtualScreen: GLint)

Gets the value for the specified pixel format attribute.

var numberOfVirtualScreens: GLint

The number of virtual screens associated with the OpenGL pixel format.

### Constants

typealias NSOpenGLPixelFormatAttribute

Pixel format attributes for OpenGL.

OpenGL Pixel Format Attributes

Pixel format attributes for OpenGL.

OpenGL Profiles

Constants that specify the functionality provided by the renderer.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol

## See Also

### Classes

class NSOpenGLView

A view that displays OpenGL content in a view.

Deprecated

class NSOpenGLContext

An object that represents an OpenGL graphics context, into which all OpenGL calls are rendered.

Deprecated

class NSOpenGLLayer

A subclass of CAOpenGLLayer that is suitable for rendering OpenGL into layers.

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

