

- VisionKit
- ImageAnalysisOverlayViewDelegate
-  overlayView(\_:liveTextButtonDidChangeToVisible:) 

Instance Method

# overlayView(\_:liveTextButtonDidChangeToVisible:)

Notifies your app when the Live Text button’s visibility changes.

macOS 13.0+

``` source
@MainActor
func overlayView(
    _ overlayView: ImageAnalysisOverlayView,
    liveTextButtonDidChangeToVisible visible: Bool
)
```

**Required** Default implementation provided.

## Parameters 

`overlayView`  

The associated overlay view for the Live Text button.

`visible`  

`true` if the Live Text button appears; otherwise, `false`.

## Default Implementations

### ImageAnalysisOverlayViewDelegate Implementations

func overlayView(ImageAnalysisOverlayView, liveTextButtonDidChangeToVisible: Bool)

A default, blank implementation for when the Live Text button appears or disappears.

## See Also

### Tracking interface changes

func overlayView(ImageAnalysisOverlayView, highlightSelectedItemsDidChange: Bool)

Notifies your app when recognized items in the image appear highlighted as a result of a person clicking or tapping the Live Text button.

**Required** Default implementation provided.

func textSelectionDidChange(ImageAnalysisOverlayView)

Notifies your app when the interaction’s text selection changes.

**Required** Default implementation provided.

