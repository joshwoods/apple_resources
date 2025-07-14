

- Vision
- ContoursObservation
-  normalizedPath 

Instance Property

# normalizedPath

The detected contours as a path object in normalized coordinates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var normalizedPath: CGPath { get }
```

## See Also

### Inspecting an observation

var contourCount: Int

The total number of detected contours.

var topLevelContours: [ContoursObservation.Contour]

An array of contours that don’t have another contour enclosing them.

