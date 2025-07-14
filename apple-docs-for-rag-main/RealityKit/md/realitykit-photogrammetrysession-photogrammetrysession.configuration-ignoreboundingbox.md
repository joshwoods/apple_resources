

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
-  ignoreBoundingBox 

Instance Property

# ignoreBoundingBox

Ignores any bounding box information embedded in the input images and instead returns all possible geometry that can be automatically estimated using the image set. The resulting mesh will likely need post-processing. Note: to recover the entire scene geometry as well as ignore the box, `isObjectMaskingEnabled` should also be set to false.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var ignoreBoundingBox: Bool
```

