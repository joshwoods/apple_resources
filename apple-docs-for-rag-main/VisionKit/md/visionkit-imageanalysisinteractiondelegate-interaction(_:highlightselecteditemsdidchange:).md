

- VisionKit
- ImageAnalysisInteractionDelegate
-  interaction(\_:highlightSelectedItemsDidChange:) 

Instance Method

# interaction(\_:highlightSelectedItemsDidChange:)

Notifies your app when recognized items in the image appear highlighted as a result of a person tapping the Live Text button.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
func interaction(
    _ interaction: ImageAnalysisInteraction,
    highlightSelectedItemsDidChange highlightSelectedItems: Bool
)
```

**Required** Default implementation provided.

## Parameters 

`interaction`  

The interaction object for which the selected item highlights change.

`highlightSelectedItems`  

A Boolean value that indicates whether highlights appear.

## Default Implementations

### ImageAnalysisInteractionDelegate Implementations

func interaction(ImageAnalysisInteraction, highlightSelectedItemsDidChange: Bool)

A default, blank implementation for when recognized items in the image appear highlighted as a result of a person tapping the Live Text button.

## See Also

### Tracking interface changes

func interaction(ImageAnalysisInteraction, liveTextButtonDidChangeToVisible: Bool)

Notifies your app when the Live Text button’s visibility changes.

**Required** Default implementation provided.

func textSelectionDidChange(ImageAnalysisInteraction)

Notifies your app when the interaction’s text selection changes.

**Required** Default implementation provided.

