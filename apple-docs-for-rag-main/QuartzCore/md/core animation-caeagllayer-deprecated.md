

- Core Animation
-  CAEAGLLayer Deprecated

Class

# CAEAGLLayer

A layer that supports drawing OpenGL content in iOS and tvOS applications.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
class CAEAGLLayer
```

Deprecated

OpenGLES is deprecated

## Overview

If you plan to use OpenGL for your rendering, use this class as the backing layer for your views by returning it from your view’s layerClass class method. The returned CAEAGLLayer object is a wrapper for a Core Animation surface that is fully compatible with OpenGL ES function calls.

Prior to designating the layer’s associated view as the render target for a graphics context, you can change the rendering attributes you want using the drawableProperties property. This property lets you configure the color format for the rendering surface and whether the surface retains its contents. For a list of keys (and corresponding values) you can include in this dictionary (along with their default values), see the EAGLDrawable.

Because an OpenGL ES rendering surface is presented to the user using Core Animation, any effects and animations you apply to the layer affect the 3D content you render. However, for best performance, do the following:

- Set the layer’s opaque attribute to `TRUE`.

- Set the layer bounds to match the dimensions of the display.

- Make sure the layer is not transformed.

- Avoid drawing other layers on top of the `CAEAGLLayer` object. If you must draw other, non OpenGL content, you might find the performance cost acceptable if you place transparent 2D content on top of the GL content and also make sure that the OpenGL content is opaque and not transformed.

- When drawing landscape content on a portrait display, you should rotate the content yourself rather than using the `CAEAGLLayer` transform to rotate it.

## Topics

### Accessing the Layer Properties

var drawableProperties: [String : Any]? { get set }

A dictionary of values that specify the desired characteristics of the drawable surface.

var presentsWithTransaction: Bool

A Boolean value that determines whether the layer presents its content using a Core Animation transaction.

## Relationships

### Inherits From

- CALayer

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- EAGLDrawable
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

class CAEDRMetadata

Metadata describing how extended dynamic range (EDR) values should be tone mapped.

class CAOpenGLLayer

A layer that provides a layer suitable for rendering OpenGL content.

Deprecated

class CARenderer

A layer that allows an application to render a layer tree into a Core OpenGL context.

