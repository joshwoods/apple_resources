

- VisionKit
- ImageAnalysisInteraction
-  subject(at:) 

Instance Method

# subject(at:)

Returns the subject at the given point within the interaction’s image, if one exists.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final func subject(at point: CGPoint) async -> ImageAnalysisInteraction.Subject?
```

## Parameters 

`point`  

A point in view coordinates at which to select a subject.

## Return Value

The subject that resides at `point`; or, `nil`, if no subject resides at `point`.

## Discussion

This method works for interaction types that include imageSubject.

The following code retrieves a subject image given a screen point, for instance, where a person taps:

```
let configuration = ImageAnalyzer.Configuration()
...
interaction.preferredInteractionTypes = [.imageSubject]
...
let viewPoint = /* A point in view coordinates */
if let subjectObject = try await interaction.subject(at: viewPoint) {
    if let image = subjectObject.image {
        // Do something with the subject image.
    }
}
```

## See Also

### Accessing image subjects

var subjects: Set&lt;ImageAnalysisInteraction.Subject>

The set of all subjects the framework identifies in an image.

struct Subject

An area of interest in an image that the framework identifies as a primary focal point.

func image(for: Set&lt;ImageAnalysisInteraction.Subject>) async throws -> UIImage

Provides an image asynchronously that contains the given subjects with the background removed.

