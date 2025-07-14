

- Core Animation
-  CAMetalDrawable 

Protocol

# CAMetalDrawable

A Metal drawable associated with a Core Animation layer.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
protocol CAMetalDrawable : MTLDrawable
```

## Overview

A CAMetalLayer instance owns any instance that implements this protocol. Don’t implement this protocol yourself. See the CAMetalLayer reference for information on how to request drawable objects.

## Topics

### Getting the Drawable’s Texture

var texture: any MTLTexture

A Metal texture object that contains the drawable’s contents.

**Required**

### Getting the Owning Layer

var layer: CAMetalLayer

The layer that owns this drawable object.

**Required**

## Relationships

### Inherits From

- MTLDrawable
- NSObjectProtocol

## See Also

### Metal and OpenGL

class CAMetalLayer

A Core Animation layer that Metal can render into, typically displayed onscreen.

class CAEAGLLayer

A layer that supports drawing OpenGL content in iOS and tvOS applications.

Deprecated

class CAEDRMetadata

Metadata describing how extended dynamic range (EDR) values should be tone mapped.

class CAOpenGLLayer

A layer that provides a layer suitable for rendering OpenGL content.

Deprecated

class CARenderer

A layer that allows an application to render a layer tree into a Core OpenGL context.

