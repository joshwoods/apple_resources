

- Metal
-  MTLTextureUsage 

Structure

# MTLTextureUsage

An enumeration for the various options that determine how you can use a texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct MTLTextureUsage
```

## Mentioned in 

Optimizing Texture Data

## Overview

If a texture has multiple uses in your app, you can combine multiple usage options for that texture. After you set the texture’s usage options, you can use it only in the ways that you specified.

Metal can optimize operations for a given texture, based on its intended use. Set explicit usage options for a texture, if you know them in advance, before you use the texture. Only set usage options that correspond to a texture’s intended use.

In iOS devices with GPU family 5, Metal doesn’t apply lossless compression to a given texture if you set any of these options:

- unknown

- shaderWrite

- pixelFormatView

## Topics

### Specifying Texture Usage Options

static var unknown: MTLTextureUsage

An option for a texture whose usage is unknown.

static var shaderRead: MTLTextureUsage

An option for reading or sampling from the texture in a shader.

static var shaderWrite: MTLTextureUsage

An option for writing to the texture in a shader.

static var renderTarget: MTLTextureUsage

An option for rendering to the texture in a render pass.

static var pixelFormatView: MTLTextureUsage

An option to create texture views with a different component layout.

### Creating Texture Usage Options

init(rawValue: UInt)

Creates new, empty usage options.

### Type Properties

static var shaderAtomic: MTLTextureUsage

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

### Querying Texture Attributes

var textureType: MTLTextureType

The dimension and arrangement of the texture image data.

**Required**

var pixelFormat: MTLPixelFormat

The format of pixels in the texture.

**Required**

var width: Int

The width of the texture image for the base level mipmap, in pixels.

**Required**

var height: Int

The height of the texture image for the base level mipmap, in pixels.

**Required**

var depth: Int

The depth of the texture image for the base level mipmap, in pixels.

**Required**

var mipmapLevelCount: Int

The number of mipmap levels in the texture.

**Required**

var arrayLength: Int

The number of slices in the texture array.

**Required**

var sampleCount: Int

The number of samples in each pixel.

**Required**

var isFramebufferOnly: Bool

A Boolean value that indicates whether the texture can only be used as a render target.

**Required**

var usage: MTLTextureUsage

Options that determine how you can use the texture.

**Required**

var allowGPUOptimizedContents: Bool

A Boolean value indicating whether the GPU is allowed to adjust the contents of the texture to improve GPU performance.

**Required**

var isShareable: Bool

A Boolean indicating whether this texture can be shared with other processes.

**Required**

var swizzle: MTLTextureSwizzleChannels

The pattern that the GPU applies to pixels when you read or sample pixels from the texture.

**Required**

enum MTLTextureType

The dimension of each image, including whether multiple images are arranged into an array or a cube.

