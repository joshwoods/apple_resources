

- Core Graphics
-  CGPatternTiling 

Enumeration

# CGPatternTiling

Different methods for rendering a tiled pattern.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGPatternTiling
```

## Topics

### Constants

case noDistortion

The pattern cell is not distorted when painted.The spacing between pattern cells may vary by as much as 1 devicepixel.

case constantSpacingMinimalDistortion

Pattern cells are spaced consistently. Thepattern cell may be distorted by as much as 1 device pixel whenthe pattern is painted.

case constantSpacing

Pattern cells are spaced consistently, as with CGPatternTiling.constantSpacingMinimalDistortion.The pattern cell may be distorted additionally to permit a moreefficient implementation.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

