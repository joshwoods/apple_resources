

- CarPlay
- CPAssistantCellActionType
-  CPAssistantCellActionType.startCall 

Case

# CPAssistantCellActionType.startCall

Provides an action that uses Siri to prompt the user for a person, group, or business to call.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case startCall
```

## Discussion

Note

This action is only available in communication apps that include an Intents Extension capable of handling doc://com.apple.documentation/documentation/sirikit/instartcallintent. For more information, see Creating an Intents App Extension.

The system provides the user’s response to your app’s Intents Extension. Your app must respond by identifying the requested person, group, or business and start a voice call with them.

## See Also

### Siri Actions

case playMedia

Provides an action that uses Siri to prompt the user for media playback.

