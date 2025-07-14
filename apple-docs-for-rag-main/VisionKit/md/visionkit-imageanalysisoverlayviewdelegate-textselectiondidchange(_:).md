

- VisionKit
- ImageAnalysisOverlayViewDelegate
-  textSelectionDidChange(\_:) 

Instance Method

# textSelectionDidChange(\_:)

Notifies your app when the interaction’s text selection changes.

macOS 14.0+

``` source
@MainActor
func textSelectionDidChange(_ overlayView: ImageAnalysisOverlayView)
```

**Required** Default implementation provided.

## Parameters 

`overlayView`  

The overlay view in which the text selection changes.

## Default Implementations

### ImageAnalysisOverlayViewDelegate Implementations

func textSelectionDidChange(ImageAnalysisOverlayView)

Notifies your app when the interaction’s text selection changes.

## See Also

### Tracking interface changes

func overlayView(ImageAnalysisOverlayView, liveTextButtonDidChangeToVisible: Bool)

Notifies your app when the Live Text button’s visibility changes.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, highlightSelectedItemsDidChange: Bool)

Notifies your app when recognized items in the image appear highlighted as a result of a person clicking or tapping the Live Text button.

**Required** Default implementation provided.

