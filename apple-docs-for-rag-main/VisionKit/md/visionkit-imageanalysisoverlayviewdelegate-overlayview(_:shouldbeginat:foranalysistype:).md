

- VisionKit
- ImageAnalysisOverlayViewDelegate
-  overlayView(\_:shouldBeginAt:forAnalysisType:) 

Instance Method

# overlayView(\_:shouldBeginAt:forAnalysisType:)

Provides a Boolean value that indicates whether the interaction can begin at the given point.

macOS 13.0+

``` source
@MainActor
func overlayView(
    _ overlayView: ImageAnalysisOverlayView,
    shouldBeginAt point: CGPoint,
    forAnalysisType analysisType: ImageAnalysisOverlayView.InteractionTypes
) -> Bool
```

**Required** Default implementation provided.

## Parameters 

`overlayView`  

The overlay view for which interaction can begin.

`point`  

The point where the interaction can begin.

`analysisType`  

The type of interaction that can begin.

## Return Value

`true` if the interaction can begin; otherwise, `false`.

## Discussion

The system calls this method once for each type of interaction. The default value is `true`, which starts the interaction immediately after the image displays.

## Default Implementations

### ImageAnalysisOverlayViewDelegate Implementations

func overlayView(ImageAnalysisOverlayView, shouldBeginAt: CGPoint, forAnalysisType: ImageAnalysisOverlayView.InteractionTypes) -> Bool

Indicates whether interaction begins at the given point for the specified interaction type.

