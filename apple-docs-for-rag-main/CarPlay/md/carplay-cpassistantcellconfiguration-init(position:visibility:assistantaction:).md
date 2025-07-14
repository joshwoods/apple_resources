

- CarPlay
- CPAssistantCellConfiguration
-  init(position:visibility:assistantAction:) 

Initializer

# init(position:visibility:assistantAction:)

Creates a configuration object with the specified position, visibility, and action.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
init(
    position: CPListItem.AssistantCellPosition,
    visibility: CPListItem.AssistantCellVisibility,
    assistantAction: CPAssistantCellActionType
)
```

## Parameters 

`position`  

The position of the assistant cell in the list template. For possible values, see CPListItem.AssistantCellPosition.

`visibility`  

The visibility of the assistant cell. For possible values, see CPListItem.AssistantCellVisibility.

`assistantAction`  

The action that Siri performs when the user selects the assistant cell. For possible values, see CPAssistantCellActionType.

## Discussion

Your app doesn’t receive a callback when the user selects the assistant cell. Instead, you configure an Intents Extension to handle the type of intent you specify in `assistantAction`; audio apps must support doc://com.apple.documentation/documentation/sirikit/inplaymediaintent and communication apps must support doc://com.apple.documentation/documentation/sirikit/instartcallintent. The assistant cell is unavailable in all other app categories.

