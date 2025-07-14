

- VisionKit
- ImageAnalysisInteraction
-  subjects 

Instance Property

# subjects

The set of all subjects the framework identifies in an image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final var subjects: Set { get async }
```

## See Also

### Accessing image subjects

struct Subject

An area of interest in an image that the framework identifies as a primary focal point.

func image(for: Set&lt;ImageAnalysisInteraction.Subject>) async throws -> UIImage

Provides an image asynchronously that contains the given subjects with the background removed.

func subject(at: CGPoint) async -> ImageAnalysisInteraction.Subject?

Returns the subject at the given point within the interaction’s image, if one exists.

