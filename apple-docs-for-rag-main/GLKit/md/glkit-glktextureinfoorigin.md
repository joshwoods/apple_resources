

- GLKit
-  GLKTextureInfoOrigin 

Enumeration

# GLKTextureInfoOrigin

The location of the origin in the original source image.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
enum GLKTextureInfoOrigin
```

## Overview

The origin’s position has no effect on how the texture is loaded into the context. If you need to flip the image before loading it, your app must explicitly add the GLKTextureOriginBottomLeft key to the options dictionary provided when loading the texture.

## Topics

### Constants

case unknown

The origin of the texture is not supported.

case topLeft

The origin of the texture is in the top-left corner.

case bottomLeft

The origin of the texture is in the bottom-left corner.

### Initializers

init?(rawValue: GLint)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum GLKTextureInfoAlphaState

Values that describe the alpha information stored in a source image’s pixel data.

