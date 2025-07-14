

- SpriteKit
-  SKTextureFilteringMode 

Enumeration

# SKTextureFilteringMode

Texture filtering modes to use when the texture is drawn in a size other than its native size.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum SKTextureFilteringMode
```

## Topics

### Constants

case nearest

Each pixel is drawn using the nearest point in the texture. This mode is faster, but the results are often pixelated.

case linear

Each pixel is drawn by using a linear filter of multiple texels in the texture. This mode produces higher quality results but may be slower.

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

### Configuring a Texture’s Behavior for Scaling

var filteringMode: SKTextureFilteringMode

The filtering mode used when the size of a sprite drawn with the texture is not drawn at the texture’s native size.

var usesMipmaps: Bool

A Boolean value that indicates whether the texture attempts to generate mipmaps.

