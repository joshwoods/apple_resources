

- VisionKit
- ImageAnalysisOverlayViewDelegate
-  overlayView(\_:highlightSelectedItemsDidChange:) 

Instance Method

# overlayView(\_:highlightSelectedItemsDidChange:)

Notifies your app when recognized items in the image appear highlighted as a result of a person clicking or tapping the Live Text button.

macOS 13.0+

``` source
@MainActor
func overlayView(
    _ overlayView: ImageAnalysisOverlayView,
    highlightSelectedItemsDidChange highlightSelectedItems: Bool
)
```

**Required** Default implementation provided.

## Parameters 

`overlayView`  

The overlay view for which the selected item highlights change.

`highlightSelectedItems`  

A Boolean value that indicates whether highlights appear.

## Default Implementations

### ImageAnalysisOverlayViewDelegate Implementations

func overlayView(ImageAnalysisOverlayView, highlightSelectedItemsDidChange: Bool)

A default, blank implementation for when recognized items in the image appear highlighted as a result of a person clicking or tapping the Live Text button.

## See Also

### Tracking interface changes

func overlayView(ImageAnalysisOverlayView, liveTextButtonDidChangeToVisible: Bool)

Notifies your app when the Live Text button’s visibility changes.

**Required** Default implementation provided.

func textSelectionDidChange(ImageAnalysisOverlayView)

Notifies your app when the interaction’s text selection changes.

**Required** Default implementation provided.

