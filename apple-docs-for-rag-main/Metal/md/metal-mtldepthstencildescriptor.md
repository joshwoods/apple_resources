

- Metal
-  MTLDepthStencilDescriptor 

Class

# MTLDepthStencilDescriptor

An object that configures new MTLDepthStencilState objects.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLDepthStencilDescriptor
```

## Overview

A MTLDepthStencilDescriptor object is used to define a specific configuration of the depth and stencil stages of a rendering pipeline. To create a MTLDepthStencilDescriptor object, use standard allocation and initialization techniques.

To enable writing the depth value to a depth attachment, set the depthWriteEnabled property to true.

The depthCompareFunction property specifies how the depth test is performed. If a fragment’s depth value fails the depth test, the fragment is discarded. MTLCompareFunction.less is a commonly used value for depthCompareFunction, because fragment values that are farther away from the viewer than the pixel depth value (a previously written fragment) fail the depth test and are considered occluded by the earlier depth value.

The frontFaceStencil and backFaceStencil properties define two independent stencil descriptors: one for front-facing primitives and the other for back-facing primitives, respectively. Both properties can be set to the same MTLStencilDescriptor object.

## Topics

### Specifying Depth Operations

var depthCompareFunction: MTLCompareFunction

The comparison that is performed between a fragment’s depth value and the depth value in the attachment, which determines whether to discard the fragment.

var isDepthWriteEnabled: Bool

A Boolean value that indicates whether depth values can be written to the depth attachment.

### Specifying Stencil Descriptors for Primitives

var backFaceStencil: MTLStencilDescriptor!

The stencil descriptor for back-facing primitives.

var frontFaceStencil: MTLStencilDescriptor!

The stencil descriptor for front-facing primitives.

### Identifying Properties

var label: String?

A string that identifies this object.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Depth Testing

Calculating Primitive Visibility Using Depth Testing

Determine which pixels are visible in a scene by using a depth texture.

protocol MTLDepthStencilState

A depth and stencil state object that specifies the depth and stencil configuration and operations used in a render pass.

class MTLStencilDescriptor

An object that defines the front-facing or back-facing stencil operations of a depth and stencil state object.

