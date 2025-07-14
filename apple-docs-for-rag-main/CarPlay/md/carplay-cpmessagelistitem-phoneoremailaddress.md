

- CarPlay
- CPMessageListItem
-  phoneOrEmailAddress 

Instance Property

# phoneOrEmailAddress

The contact’s phone number or email address.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var phoneOrEmailAddress: String? { get set }
```

## Discussion

When the user selects the list item, Siri launches the message compose flow and uses this property’s value as the recipient’s contact information.

## See Also

### Managing the Message Context

var conversationIdentifier: String?

The conversation’s unique identifier.

