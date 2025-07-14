

- VisionKit
- ImageAnalysisInteractionDelegate
-  textSelectionDidChange(\_:) 

Instance Method

# textSelectionDidChange(\_:)

Notifies your app when the interaction’s text selection changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
func textSelectionDidChange(_ interaction: ImageAnalysisInteraction)
```

**Required** Default implementation provided.

## Parameters 

`interaction`  

The interaction object in which the text selection changes.

## Default Implementations

### ImageAnalysisInteractionDelegate Implementations

func textSelectionDidChange(ImageAnalysisInteraction)

A default, blank implementation for when the text selection changes.

## See Also

### Tracking interface changes

func interaction(ImageAnalysisInteraction, liveTextButtonDidChangeToVisible: Bool)

Notifies your app when the Live Text button’s visibility changes.

**Required** Default implementation provided.

func interaction(ImageAnalysisInteraction, highlightSelectedItemsDidChange: Bool)

Notifies your app when recognized items in the image appear highlighted as a result of a person tapping the Live Text button.

**Required** Default implementation provided.

