

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.State
-  UIWritingToolsCoordinator.State.inactive 

Case

# UIWritingToolsCoordinator.State.inactive

A state that indicates Writing Tools isn’t currently performing any work on your view’s content.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
case inactive
```

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Discussion

The coordinator starts in the `inactive` state, and transitions immediately to the UIWritingToolsCoordinator.State.noninteractive or UIWritingToolsCoordinator.State.interactiveResting state when someone chooses an option from the Writing Tools UI. After the coordinator finishes incorporating any changes for the current operation, it returns to the `inactive` state and waits for the person to choose a different option or dismiss the Writing Tools UI.

## See Also

### Getting the animation types

case noninteractive

A state that indicates Writing Tools is handling interactions in the system UI, instead of in your view.

case interactiveResting

A state that indicates Writing Tools is in the resting state for an inline editing experience.

case interactiveStreaming

A state that indicates Writing Tools is processing a request and incorporating changes interactively into your view.

