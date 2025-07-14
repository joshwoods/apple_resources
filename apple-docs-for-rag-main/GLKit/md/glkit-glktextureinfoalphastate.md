

- GLKit
-  GLKTextureInfoAlphaState 

Enumeration

# GLKTextureInfoAlphaState

Values that describe the alpha information stored in a source image’s pixel data.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
enum GLKTextureInfoAlphaState
```

## Topics

### Constants

case none

Indicates that the texture has no alpha information.

case nonPremultiplied

Indicates that the color values in the texture were not premultiplied by the alpha value.

case premultiplied

Indicates that the color values in the texture have already been premultiplied by the alpha value.

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

enum GLKTextureInfoOrigin

The location of the origin in the original source image.

