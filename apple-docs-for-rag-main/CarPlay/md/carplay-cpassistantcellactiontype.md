

- CarPlay
-  CPAssistantCellActionType 

Enumeration

# CPAssistantCellActionType

The supported Siri actions of the assistant cell.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
enum CPAssistantCellActionType
```

## Topics

### Siri Actions

case playMedia

Provides an action that uses Siri to prompt the user for media playback.

case startCall

Provides an action that uses Siri to prompt the user for a person, group, or business to call.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Configuration Attributes

var position: CPListItem.AssistantCellPosition

The position of the assistant cell in the list template.

var visibility: CPListItem.AssistantCellVisibility

The visibility of the assistant cell in the list template.

var assistantAction: CPAssistantCellActionType

The action that Siri performs when the user selects the assistant cell.

