

- Metal
-  MTLDepthStencilState 

Protocol

# MTLDepthStencilState

A depth and stencil state object that specifies the depth and stencil configuration and operations used in a render pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLDepthStencilState : NSObjectProtocol
```

## Overview

The MTLDepthStencilState protocol defines the interface for a lightweight object used to encode how a graphics rendering pass should perform depth and stencil operations. The MTLRenderCommandEncoder uses a MTLDepthStencilState object to set the depth and stencil state for a rendering pass.

Do not use standard allocation and initialization techniques to create a MTLDepthStencilState object. To create a MTLDepthStencilState object:

1.  Create a MTLDepthStencilDescriptor object that defines the operations you want the rendering pass to use.

2.  Then call the makeDepthStencilState(descriptor:) method of MTLDevice to create a MTLDepthStencilState object.

Typically, you create MTLDepthStencilState objects when your app is first initialized and then reuse them throughout the lifetime of your app.

## Topics

### Identifying Properties

var device: any MTLDevice

The device from which this state object was created.

**Required**

var label: String?

A string that identifies this object.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Depth Testing

Calculating Primitive Visibility Using Depth Testing

Determine which pixels are visible in a scene by using a depth texture.

class MTLDepthStencilDescriptor

An object that configures new MTLDepthStencilState objects.

class MTLStencilDescriptor

An object that defines the front-facing or back-facing stencil operations of a depth and stencil state object.

