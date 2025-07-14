

- Metal
-  MTLBlitOption 

Structure

# MTLBlitOption

The options that enable behavior for some blit operations.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct MTLBlitOption
```

## Topics

### Depth and Stencil Buffer Options

static var depthFromDepthStencil: MTLBlitOption

A blit option that copies the depth portion of a combined depth and stencil texture to or from a buffer.

static var stencilFromDepthStencil: MTLBlitOption

A blit option that copies the stencil portion of a combined depth and stencil texture to or from a buffer.

### Texture Compression Options

static var rowLinearPVRTC: MTLBlitOption

A blit option that copies PVRTC data between a texture and a buffer.

### Clearing Options

init(rawValue: UInt)

Creates a blit option from a raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Encoding a Blit Pass

protocol MTLBlitCommandEncoder

An interface you can use to encode GPU commands that copy and modify the underlying memory of various Metal resources.

