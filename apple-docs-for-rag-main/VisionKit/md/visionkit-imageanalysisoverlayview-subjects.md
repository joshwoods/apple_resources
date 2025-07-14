

- VisionKit
- ImageAnalysisOverlayView
-  subjects 

Instance Property

# subjects

The set of all subjects the framework identifies in an image.

macOS 13.0+

``` source
@MainActor
final var subjects: Set { get async }
```

## See Also

### Accessing image subjects

struct Subject

An area of interest in an image that the framework identifies as a primary focal point.

func image(for: Set&lt;ImageAnalysisOverlayView.Subject>) async throws -> NSImage

Provides an image asynchronously that contains the given subjects with the background removed.

func subject(at: CGPoint) async -> ImageAnalysisOverlayView.Subject?

Returns the subject at the given point within the overlay view’s image, if one exists.

