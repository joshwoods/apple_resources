

- AppKit
- NSImage
-  matchesOnMultipleResolution 

Instance Property

# matchesOnMultipleResolution

A Boolean value that indicates whether image representations whose resolution is an integral multiple of the device resolution are a match.

macOS

``` source
var matchesOnMultipleResolution: Bool { get set }
```

## Discussion

When this property is set to false, only image representations whose resolution is exactly the same as the device resolution are matches. If the property is set to true and multiple image representations fit this criteria, the one whose resolution is closest to the device resolution is chosen.

The default value is true.

## See Also

### Setting the Representation Selection Criteria for Images

var prefersColorMatch: Bool

A Boolean value that indicates whether the image prefers to choose image representations using color-matching or resolution-matching.

var usesEPSOnResolutionMismatch: Bool

A Boolean value that indicates whether EPS representations are preferred when no other representations match the resolution of the device.

