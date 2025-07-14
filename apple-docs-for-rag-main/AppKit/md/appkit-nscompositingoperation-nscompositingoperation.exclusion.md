

- AppKit
- NSCompositingOperation
-  NSCompositingOperation.exclusion 

Case

# NSCompositingOperation.exclusion

Subtracts the darker value from the lighter value, except lower in contrast.

macOS 10.10+

``` source
case exclusion
```

## See Also

### Operations for Compositing

case clear

Transparency everywhere.

case copy

The source image.

case sourceOver

The source image wherever it is opaque, and the destination image elsewhere.

case sourceIn

The source image wherever both images are opaque, and transparent elsewhere.

case sourceOut

The source image wherever it is opaque and the destination image is transparent, and transparent elsewhere.

case sourceAtop

The source image wherever both images are opaque, the destination image wherever it is opaque but the source image is transparent, and transparent elsewhere

case destinationOver

The destination image wherever it is opaque, and the source image elsewhere.

case destinationIn

The destination image wherever both images are opaque, and transparent elsewhere.

case destinationOut

The destination image wherever it is opaque and the source image is transparent, and transparent elsewhere.

case destinationAtop

The destination image wherever both images are opaque, the source image wherever it is opaque and the destination image is transparent, and transparent elsehwere.

case xor

Exclusive OR of the source and destination images.

case plusDarker

The sum of the source and destination images, with color values approach 0 as a limit.

case plusLighter

The sum of the source and destination images, with color values approach 1 as a limit.

case multiply

The source color is multiplied by the destination color.

case screen

Multiplies the complement of the destination and source color values, and then complements the result.

