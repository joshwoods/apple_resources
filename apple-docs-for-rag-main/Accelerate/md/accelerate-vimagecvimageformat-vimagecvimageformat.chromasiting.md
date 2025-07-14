

- Accelerate
- vImageCVImageFormat
-  vImageCVImageFormat.ChromaSiting 

Enumeration

# vImageCVImageFormat.ChromaSiting

Constants that specify the chrominance siting of a Core Video image format.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
enum ChromaSiting
```

## Topics

### Chrominance siting constants

case top

The chrominance sample is horizontally centered, but co-sited with the top row of luminance samples.

case topLeft

The chrominance sample is co-sited with the top-left luminance sample.

case bottom

The chrominance sample is horizontally centered, but co-sited with the bottom row of luminance samples.

case bottomLeft

The chrominance sample is co-sited with the bottom-left luminance sample.

case left

The chrominance sample is horizontally co-sited with the left column of luminance samples, but centered vertically.

case center

The chrominance sample is fully centered.

case dv420

The Cr and Cb samples are alternately co-sited with the left luminance samples of the same field.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Supporting types

enum Format

Constants that specify the format of a Core Video image format.

