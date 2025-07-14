

- AppKit
- NSImage
-  usesEPSOnResolutionMismatch 

Instance Property

# usesEPSOnResolutionMismatch

A Boolean value that indicates whether EPS representations are preferred when no other representations match the resolution of the device.

macOS

``` source
var usesEPSOnResolutionMismatch: Bool { get set }
```

## Discussion

The default value is false.

## See Also

### Setting the Representation Selection Criteria for Images

var prefersColorMatch: Bool

A Boolean value that indicates whether the image prefers to choose image representations using color-matching or resolution-matching.

var matchesOnMultipleResolution: Bool

A Boolean value that indicates whether image representations whose resolution is an integral multiple of the device resolution are a match.

