

- CarPlay
- CPMessageListItem
-  init(conversationIdentifier:text:leadingConfiguration:trailingConfiguration:detailText:trailingText:) 

Initializer

# init(conversationIdentifier:text:leadingConfiguration:trailingConfiguration:detailText:trailingText:)

Creates a list item that represents an existing conversation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    conversationIdentifier: String,
    text: String,
    leadingConfiguration: CPMessageListItemLeadingConfiguration,
    trailingConfiguration: CPMessageListItemTrailingConfiguration?,
    detailText: String?,
    trailingText: String?
)
```

## Parameters 

`conversationIdentifier`  

Your app’s unique identifier for the conversation. Siri passes this value to your app when the user selects the list item.

`text`  

The conversation’s content. Siri speaks this when the user selects the list item.

`leadingConfiguration`  

The configuration that describes the visual elements of the list item’s leading region.

`trailingConfiguration`  

The configuration that describes the visual elements of the list item’s trailing region.

`detailText`  

The list item’s secondary text.

`trailingText`  

Supplementary text that the list item’s trailing region displays.

## See Also

### Creating a Message List Item

init(fullName: String, phoneOrEmailAddress: String, leadingConfiguration: CPMessageListItemLeadingConfiguration, trailingConfiguration: CPMessageListItemTrailingConfiguration?, detailText: String?, trailingText: String?)

Creates a list item that represents a contact.

