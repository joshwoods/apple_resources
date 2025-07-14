

- VisionKit
- ImageAnalysisOverlayView
-  beginSubjectAnalysisIfNecessary() 

Instance Method

# beginSubjectAnalysisIfNecessary()

Begins subject analysis on the overlay view’s image.

macOS 13.0+

``` source
@MainActor
final func beginSubjectAnalysisIfNecessary()
```

## Discussion

Subject analysis begins automatically without calling this method moments after the overlay view’s image displays onscreen. The framework ignores calls to this method if subject analysis is already in progress or complete.

Note

For subject analysis to begin, preferredInteractionTypes needs to contain a subject-related option, such as automatic, imageSubject, or visualLookUp.

## See Also

### Managing image subjects

var highlightedSubjects: Set&lt;ImageAnalysisOverlayView.Subject>

All highlighted subjects in the overlay view’s image.

