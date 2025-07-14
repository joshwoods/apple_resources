

- Messages
- MSMessage
-  init() 

Initializer

# init()

Initializes a new message that is not part of a session.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
init()
```

## Return Value

A newly initialized message.

## Discussion

Use this initializer to create a new message that transmits app data, but is not updatable. When the recipient selects the message, the recipient’s app extension launches and receives the message object, but it cannot update the message.

## See Also

### Creating Messages

init(session: MSSession)

Initializes a new message that is part of the provided session.

