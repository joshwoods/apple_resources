

- VisionKit
- ImageAnalysisInteractionDelegate
-  interaction(\_:liveTextButtonDidChangeToVisible:) 

Instance Method

# interaction(\_:liveTextButtonDidChangeToVisible:)

Notifies your app when the Live Text button’s visibility changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
func interaction(
    _ interaction: ImageAnalysisInteraction,
    liveTextButtonDidChangeToVisible visible: Bool
)
```

**Required** Default implementation provided.

## Parameters 

`interaction`  

The interaction object for which the Live Text button appears.

`visible`  

`true` if the Live Text button appears; otherwise,`false`.

## Default Implementations

### ImageAnalysisInteractionDelegate Implementations

func interaction(ImageAnalysisInteraction, liveTextButtonDidChangeToVisible: Bool)

A default, blank implementation for when the Live Text button appears or disappears.

## See Also

### Tracking interface changes

func interaction(ImageAnalysisInteraction, highlightSelectedItemsDidChange: Bool)

Notifies your app when recognized items in the image appear highlighted as a result of a person tapping the Live Text button.

**Required** Default implementation provided.

func textSelectionDidChange(ImageAnalysisInteraction)

Notifies your app when the interaction’s text selection changes.

**Required** Default implementation provided.

