

- MailKit
- MEExtension
-  handlerForMessageActions() 

Instance Method

# handlerForMessageActions()

Returns an object that performs actions on mail messages as the system downloads them.

macOS 12.0+

``` source
@MainActor
optional func handlerForMessageActions() -> any MEMessageActionHandler
```

## Return Value

An object that performs actions on mail messages.

## Discussion

Tip

Message action handlers typically don’t need any additional state to determine the actions to take on messages. Therefore, using a singleton handler instance is appropriate.

