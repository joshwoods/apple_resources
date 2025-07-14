

- VisionKit
- ImageAnalysisOverlayView
-  subject(at:) 

Instance Method

# subject(at:)

Returns the subject at the given point within the overlay view’s image, if one exists.

macOS 13.0+

``` source
@MainActor
final func subject(at point: CGPoint) async -> ImageAnalysisOverlayView.Subject?
```

## Parameters 

`point`  

A point in view coordinates at which to select a subject.

## Return Value

The subject that resides at `point`; or, `nil`, if no subject resides at `point`.

## Discussion

This method works for interaction types that include imageSubject.

The following code retrieves a subject image given a screen point, for instance, where a person clicks:

```
let configuration = ImageAnalyzer.Configuration()
...
overlayView.preferredInteractionTypes = [.imageSubject]
...
let viewPoint = /* A point in view coordinates */
if let subjectObject = try await overlayView.subject(at: viewPoint) {
    if let image = subjectObject.image {
        // Do something with the subject image.
    }
}
```

## See Also

### Accessing image subjects

var subjects: Set&lt;ImageAnalysisOverlayView.Subject>

The set of all subjects the framework identifies in an image.

struct Subject

An area of interest in an image that the framework identifies as a primary focal point.

func image(for: Set&lt;ImageAnalysisOverlayView.Subject>) async throws -> NSImage

Provides an image asynchronously that contains the given subjects with the background removed.

