

- AppKit
- NSWritingToolsCoordinator
- NSWritingToolsCoordinator.State
-  NSWritingToolsCoordinator.State.noninteractive 

Case

# NSWritingToolsCoordinator.State.noninteractive

A state that indicates Writing Tools is handling interactions in the system UI, instead of in your view.

macOS 15.2+

``` source
case noninteractive
```

## Mentioned in 

Adding Writing Tools support to a custom AppKit view

## Discussion

Writing Tools transitions to this state when the coordinator uses the NSWritingToolsBehavior.limited experience or when someone chooses an option that displays its results in the Writing Tools UI. When the person accepts the changes from the tool or dismisses the Writing Tools UI, the coordinator returns to the NSWritingToolsCoordinator.State.inactive state. If the person discards the change and selects a tool with an interactive experience instead, the coordinator transitions to the NSWritingToolsCoordinator.State.interactiveResting state.

## See Also

### Getting the animation types

case inactive

A state that indicates Writing Tools isn’t currently performing any work on your view’s content.

case interactiveResting

A state that indicates Writing Tools is in the resting state for an inline editing experience.

case interactiveStreaming

A state that indicates Writing Tools is processing a request and incorporating changes interactively into your view.

