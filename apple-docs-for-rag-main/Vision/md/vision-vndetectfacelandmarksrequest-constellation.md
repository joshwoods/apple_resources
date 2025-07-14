

- Vision
- VNDetectFaceLandmarksRequest
-  constellation 

Instance Property

# constellation

A variable that describes how a face landmarks request orders or enumerates the resulting features.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var constellation: VNRequestFaceLandmarksConstellation { get set }
```

## Discussion

Set this variable to one of the supported constellation types detailed in VNRequestFaceLandmarksConstellation. The default value is VNRequestFaceLandmarksConstellation.constellationNotDefined.

## See Also

### Locating Face Landmarks

enum VNRequestFaceLandmarksConstellation

An enumeration of face landmarks in a constellation object.

