

- Vision
- ContoursObservation
-  topLevelContours 

Instance Property

# topLevelContours

An array of contours that don’t have another contour enclosing them.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var topLevelContours: [ContoursObservation.Contour] { get }
```

## Discussion

This array constitutes the top of the contour hierarchy. You can iterate over each Contour instance to determine its children.

## See Also

### Inspecting an observation

var contourCount: Int

The total number of detected contours.

var normalizedPath: CGPath

The detected contours as a path object in normalized coordinates.

