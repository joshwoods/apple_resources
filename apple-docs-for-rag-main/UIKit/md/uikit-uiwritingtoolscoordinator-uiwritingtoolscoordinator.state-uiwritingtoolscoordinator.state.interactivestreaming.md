

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.State
-  UIWritingToolsCoordinator.State.interactiveStreaming 

Case

# UIWritingToolsCoordinator.State.interactiveStreaming

A state that indicates Writing Tools is processing a request and incorporating changes interactively into your view.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
case interactiveStreaming
```

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Discussion

The coordinator transitions swiftly from the UIWritingToolsCoordinator.State.interactiveResting state to this state at the start of an operation. In this state, the coordinator submits the request for processing and delivers the results back to your view. When the coordinator finishes delivering the results, it transitions back to the UIWritingToolsCoordinator.State.interactiveResting state.

## See Also

### Getting the animation types

case inactive

A state that indicates Writing Tools isn’t currently performing any work on your view’s content.

case noninteractive

A state that indicates Writing Tools is handling interactions in the system UI, instead of in your view.

case interactiveResting

A state that indicates Writing Tools is in the resting state for an inline editing experience.

