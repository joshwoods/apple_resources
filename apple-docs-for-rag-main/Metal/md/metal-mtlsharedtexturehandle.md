

- Metal
-  MTLSharedTextureHandle 

Class

# MTLSharedTextureHandle

A texture handle that can be shared across process address space boundaries.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.14+tvOS 13.0+visionOS 1.0+

``` source
class MTLSharedTextureHandle
```

## Overview

`MTLSharedTextureHandle` objects may be passed between processes using XPC connections and then used to create a reference to the texture in another process. The texture in the other process must be created using the same MTLDevice on which the shared texture was originally created. To identify which device it was created on, you can use the device property of the `MTLSharedTextureHandle` object.

## Topics

### Identifying the Shared Texture Handle

var device: any MTLDevice

The device object that created the texture.

var label: String?

A string that identifies the texture.

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
- NSSecureCoding

## See Also

### Texture Basics

Understanding Color-Renderable Pixel Format Sizes

Know the size limits of color render targets in Apple GPUs based on the target’s pixel format.

Optimizing Texture Data

Optimize a texture’s data to improve GPU or CPU access.

protocol MTLTexture

A resource that holds formatted image data.

enum MTLTextureCompressionType

class MTLTextureDescriptor

An object that you use to configure new Metal texture objects.

class MTKTextureLoader

An object that creates textures from existing data in common image formats.

enum MTLPixelFormat

The data formats that describe the organization and characteristics of individual pixels in a texture.

