

- Vision
- ContoursObservation
-  contourCount 

Instance Property

# contourCount

The total number of detected contours.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var contourCount: Int { get }
```

## Discussion

Use this value to determine the number of indices available for calling contourAtIndex(_:).

## See Also

### Inspecting an observation

var normalizedPath: CGPath

The detected contours as a path object in normalized coordinates.

var topLevelContours: [ContoursObservation.Contour]

An array of contours that don’t have another contour enclosing them.

