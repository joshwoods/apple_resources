

- VisionKit
- ImageAnalysisInteractionDelegate
-  interaction(\_:shouldBeginAt:for:) 

Instance Method

# interaction(\_:shouldBeginAt:for:)

Provides a Boolean value that indicates whether the interaction can begin at the given point.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
func interaction(
    _ interaction: ImageAnalysisInteraction,
    shouldBeginAt point: CGPoint,
    for interactionType: ImageAnalysisInteraction.InteractionTypes
) -> Bool
```

**Required** Default implementation provided.

## Parameters 

`interaction`  

The object for which interaction can begin.

`point`  

The point where the interaction can begin.

`interactionType`  

The type of interaction that can begin.

## Return Value

`true` if the interaction can begin; otherwise, `false`.

## Discussion

The system calls this method once for each type of interaction. The default value is `true`, which starts the interaction immediately after the image displays.

## Default Implementations

### ImageAnalysisInteractionDelegate Implementations

func interaction(ImageAnalysisInteraction, shouldBeginAt: CGPoint, for: ImageAnalysisInteraction.InteractionTypes) -> Bool

A default implementation that indicates that the interaction begins.

