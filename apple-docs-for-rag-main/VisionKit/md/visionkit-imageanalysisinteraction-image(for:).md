

- VisionKit
- ImageAnalysisInteraction
-  image(for:) 

Instance Method

# image(for:)

Provides an image asynchronously that contains the given subjects with the background removed.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final func image(for subjects: Set) async throws -> UIImage
```

## Parameters 

`subjects`  

An array of subjects to include in the image.

## Discussion

If one or more subjects fail to produce an image, the method throws ImageAnalysisInteraction.SubjectUnavailable.imageUnavailable.

## See Also

### Accessing image subjects

var subjects: Set&lt;ImageAnalysisInteraction.Subject>

The set of all subjects the framework identifies in an image.

struct Subject

An area of interest in an image that the framework identifies as a primary focal point.

func subject(at: CGPoint) async -> ImageAnalysisInteraction.Subject?

Returns the subject at the given point within the interaction’s image, if one exists.

