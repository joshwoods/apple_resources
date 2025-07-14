

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.State
-  UIWritingToolsCoordinator.State.noninteractive 

Case

# UIWritingToolsCoordinator.State.noninteractive

A state that indicates Writing Tools is handling interactions in the system UI, instead of in your view.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
case noninteractive
```

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Discussion

Writing Tools transitions to this state when the coordinator uses the UIWritingToolsBehavior.limited experience or when someone chooses an option that displays its results in the Writing Tools UI. When the person accepts the changes from the tool or dismisses the Writing Tools UI, the coordinator returns to the UIWritingToolsCoordinator.State.inactive state. If the person discards the change and selects a tool with an interactive experience instead, the coordinator transitions to the UIWritingToolsCoordinator.State.interactiveResting state.

## See Also

### Getting the animation types

case inactive

A state that indicates Writing Tools isn’t currently performing any work on your view’s content.

case interactiveResting

A state that indicates Writing Tools is in the resting state for an inline editing experience.

case interactiveStreaming

A state that indicates Writing Tools is processing a request and incorporating changes interactively into your view.

