

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.State
-  UIWritingToolsCoordinator.State.interactiveResting 

Case

# UIWritingToolsCoordinator.State.interactiveResting

A state that indicates Writing Tools is in the resting state for an inline editing experience.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
case interactiveResting
```

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Discussion

When someone initially selects a tool with an interactive experience, the coordinator transitions briefly to this state and starts the operation. The coordinator transitions swiftly to the UIWritingToolsCoordinator.State.interactiveStreaming state when it submits the request and delivers the results to your view. When it finishes delivering the results, it transitions back to the `interactiveResting` state and awaits further commands. If the person accepts the changes or dismisses the Writing Tools UI, the coordinator transitions from this state to the UIWritingToolsCoordinator.State.inactive state.

## See Also

### Getting the animation types

case inactive

A state that indicates Writing Tools isn’t currently performing any work on your view’s content.

case noninteractive

A state that indicates Writing Tools is handling interactions in the system UI, instead of in your view.

case interactiveStreaming

A state that indicates Writing Tools is processing a request and incorporating changes interactively into your view.

