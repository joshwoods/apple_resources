

- CarPlay
- CPMessageListItem
-  init(fullName:phoneOrEmailAddress:leadingConfiguration:trailingConfiguration:detailText:trailingText:) 

Initializer

# init(fullName:phoneOrEmailAddress:leadingConfiguration:trailingConfiguration:detailText:trailingText:)

Creates a list item that represents a contact.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    fullName: String,
    phoneOrEmailAddress: String,
    leadingConfiguration: CPMessageListItemLeadingConfiguration,
    trailingConfiguration: CPMessageListItemTrailingConfiguration?,
    detailText: String?,
    trailingText: String?
)
```

## Parameters 

`fullName`  

The contact’s full name. The list item displays this value as its primary content. Siri speaks this when the user selects the list item.

`phoneOrEmailAddress`  

The phone number or email address that Siri uses when launching the compose message flow.

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

init(conversationIdentifier: String, text: String, leadingConfiguration: CPMessageListItemLeadingConfiguration, trailingConfiguration: CPMessageListItemTrailingConfiguration?, detailText: String?, trailingText: String?)

Creates a list item that represents an existing conversation.

