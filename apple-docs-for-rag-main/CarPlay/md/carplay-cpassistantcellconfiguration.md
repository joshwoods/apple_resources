

- CarPlay
-  CPAssistantCellConfiguration 

Class

# CPAssistantCellConfiguration

An object that provides the configuration attributes for the assistant cell.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
class CPAssistantCellConfiguration
```

## Overview

An audio or communication CarPlay app can choose to display an *assistant cell* in a list template that allows the user to interact with the app using Siri. You create an instance of this configuration object that describes the position, visibility, and supported Siri intent, and provide that to your app’s list template using the init(title:sections:assistantCellConfiguration:) initializer or the assistantCellConfiguration property.

Your app must include an Intents Extension that handles the intent corresponding to the action you specify in the assistantAction property; audio apps must support doc://com.apple.documentation/documentation/sirikit/inplaymediaintent and communication apps must support doc://com.apple.documentation/documentation/sirikit/instartcallintent. For more information, see Creating an Intents App Extension.

## Topics

### Creating an Assistant Cell Configuration

init(position: CPListItem.AssistantCellPosition, visibility: CPListItem.AssistantCellVisibility, assistantAction: CPAssistantCellActionType)

Creates a configuration object with the specified position, visibility, and action.

### Getting the Configuration Attributes

var position: CPListItem.AssistantCellPosition

The position of the assistant cell in the list template.

var visibility: CPListItem.AssistantCellVisibility

The visibility of the assistant cell in the list template.

var assistantAction: CPAssistantCellActionType

The action that Siri performs when the user selects the assistant cell.

enum CPAssistantCellActionType

The supported Siri actions of the assistant cell.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Managing the Assistant Cell

var assistantCellConfiguration: CPAssistantCellConfiguration?

The object that provides the configuration attributes for the assistant cell.

