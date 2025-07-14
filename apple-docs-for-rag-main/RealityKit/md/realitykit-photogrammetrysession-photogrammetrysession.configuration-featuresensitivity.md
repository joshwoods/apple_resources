

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
-  featureSensitivity 

Instance Property

# featureSensitivity

The precision of landmark detection.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var featureSensitivity: PhotogrammetrySession.Configuration.FeatureSensitivity
```

## Discussion

The photogrammetry process relies on finding identifiable landmarks in the overlap between images. Landmarks can be hard to identify if the images don’t have enough contrast, aren’t in focus, or if the object is all one color and lacks surface detail.

When featureSensitivity is set to PhotogrammetrySession.Configuration.FeatureSensitivity.high, it instructs RealityKit to search an image for landmarks using an algorithm that analyzes an image closely and in detail. This slower, more sensitive process can produce an accurate 3D object even when landmarks are difficult to discern.

## See Also

### Configuring feature sensitivity

enum FeatureSensitivity

The sensitivity to sample landmarks.

