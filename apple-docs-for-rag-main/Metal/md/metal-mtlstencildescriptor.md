

- Metal
-  MTLStencilDescriptor 

Class

# MTLStencilDescriptor

An object that defines the front-facing or back-facing stencil operations of a depth and stencil state object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLStencilDescriptor
```

## Overview

A stencil test is a comparison between a masked reference value and a masked value stored in a stencil attachment. (A value is *masked* by performing a logical AND operation on it with the readMask value.) The MTLStencilDescriptor object defines how to update the contents of the stencil attachment, based on the results of the stencil test and the depth test.

The stencilCompareFunction property defines the stencil test. The stencilFailureOperation, depthFailureOperation, and depthStencilPassOperation properties specify what to do to a stencil value stored in the stencil attachment for three different test outcomes: if the stencil test fails, if the stencil test passes and the depth test fails, or if both stencil and depth tests succeed, respectively. writeMask determines which stencil bits can be modified as the result of a stencil operation.

## Topics

### Specifying Stencil Functions and Operations

var stencilFailureOperation: MTLStencilOperation

The operation that is performed to update the values in the stencil attachment when the stencil test fails.

var depthFailureOperation: MTLStencilOperation

The operation that is performed to update the values in the stencil attachment when the stencil test passes, but the depth test fails.

var depthStencilPassOperation: MTLStencilOperation

The operation that is performed to update the values in the stencil attachment when both the stencil test and the depth test pass.

var stencilCompareFunction: MTLCompareFunction

The comparison that is performed between the masked reference value and a masked value in the stencil attachment.

### Specifying Stencil Bit Mask Properties

var readMask: UInt32

A bitmask that determines from which bits that stencil comparison tests can read.

var writeMask: UInt32

A bitmask that determines to which bits that stencil operations can write.

### Constants

enum MTLStencilOperation

The operation performed on a currently stored stencil value when a comparison test passes or fails.

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

class MTLDepthStencilDescriptor

An object that configures new MTLDepthStencilState objects.

