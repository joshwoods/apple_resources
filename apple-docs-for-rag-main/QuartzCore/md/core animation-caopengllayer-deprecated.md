

- Core Animation
-  CAOpenGLLayer Deprecated

Class

# CAOpenGLLayer

A layer that provides a layer suitable for rendering OpenGL content.

Mac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.14Deprecated

``` source
class CAOpenGLLayer
```

Deprecated

OpenGL is deprecated

## Overview

To provide OpenGL content you subclass `CAOpenGLLayer` and override draw(inCGLContext:pixelFormat:forLayerTime:displayTime:). You can specify that the OpenGL content is static by setting the isAsynchronous property to false.

## Topics

### Determining Layer Properties

var colorspace: CGColorSpace?

The layer’s colorspace in Core Graphics.

var wantsExtendedDynamicRangeContent: Bool

Tells whether or not the layer supports content with extended dynamic range.

### Drawing Layer Content

var isAsynchronous: Bool

Determines when the contents of the layer are updated.

func canDraw(inCGLContext: CGLContextObj, pixelFormat: CGLPixelFormatObj, forLayerTime: CFTimeInterval, displayTime: UnsafePointer&lt;CVTimeStamp>?) -> Bool

Returns whether the receiver should draw OpenGL content for the specified time.

func draw(inCGLContext: CGLContextObj, pixelFormat: CGLPixelFormatObj, forLayerTime: CFTimeInterval, displayTime: UnsafePointer&lt;CVTimeStamp>?)

Draws the OpenGL content for the specified time.

### Managing Pixel Format

func copyCGLPixelFormat(forDisplayMask: UInt32) -> CGLPixelFormatObj

Returns the OpenGL pixel format suitable for rendering to the set of displays specified by the display mask.

func releaseCGLPixelFormat(CGLPixelFormatObj)

Releases the specified OpenGL pixel format object.

### Managing the Rendering Context

func copyCGLContext(forPixelFormat: CGLPixelFormatObj) -> CGLContextObj

Returns the rendering context the receiver requires for the specified pixel format.

func releaseCGLContext(CGLContextObj)

Releases the specified rendering context.

## Relationships

### Inherits From

- CALayer

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

### Metal and OpenGL

class CAMetalLayer

A Core Animation layer that Metal can render into, typically displayed onscreen.

protocol CAMetalDrawable

A Metal drawable associated with a Core Animation layer.

class CAEAGLLayer

A layer that supports drawing OpenGL content in iOS and tvOS applications.

Deprecated

class CAEDRMetadata

Metadata describing how extended dynamic range (EDR) values should be tone mapped.

class CARenderer

A layer that allows an application to render a layer tree into a Core OpenGL context.

