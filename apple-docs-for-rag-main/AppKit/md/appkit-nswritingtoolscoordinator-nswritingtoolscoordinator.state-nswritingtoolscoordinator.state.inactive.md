

- AppKit
- NSWritingToolsCoordinator
- NSWritingToolsCoordinator.State
-  NSWritingToolsCoordinator.State.inactive 

Case

# NSWritingToolsCoordinator.State.inactive

A state that indicates Writing Tools isn’t currently performing any work on your view’s content.

macOS 15.2+

``` source
case inactive
```

## Mentioned in 

Adding Writing Tools support to a custom AppKit view

## Discussion

The coordinator starts in the `inactive` state, and transitions immediately to the NSWritingToolsCoordinator.State.noninteractive or NSWritingToolsCoordinator.State.interactiveResting state when someone chooses an option from the Writing Tools UI. After the coordinator finishes incorporating any changes for the current operation, it returns to the `inactive` state and waits for the person to choose a different option or dismiss the Writing Tools UI.

## See Also

### Getting the animation types

case noninteractive

A state that indicates Writing Tools is handling interactions in the system UI, instead of in your view.

case interactiveResting

A state that indicates Writing Tools is in the resting state for an inline editing experience.

case interactiveStreaming

A state that indicates Writing Tools is processing a request and incorporating changes interactively into your view.

