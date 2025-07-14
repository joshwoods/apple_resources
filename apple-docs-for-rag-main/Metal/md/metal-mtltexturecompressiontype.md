

- Metal
-  MTLTextureCompressionType 

Enumeration

# MTLTextureCompressionType

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.5+tvOS 16.0+visionOS 1.0+

``` source
enum MTLTextureCompressionType
```

## Topics

### Enumeration Cases

case lossless

case lossy

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Texture Basics

Understanding Color-Renderable Pixel Format Sizes

Know the size limits of color render targets in Apple GPUs based on the target’s pixel format.

Optimizing Texture Data

Optimize a texture’s data to improve GPU or CPU access.

protocol MTLTexture

A resource that holds formatted image data.

class MTLTextureDescriptor

An object that you use to configure new Metal texture objects.

class MTKTextureLoader

An object that creates textures from existing data in common image formats.

class MTLSharedTextureHandle

A texture handle that can be shared across process address space boundaries.

enum MTLPixelFormat

The data formats that describe the organization and characteristics of individual pixels in a texture.

