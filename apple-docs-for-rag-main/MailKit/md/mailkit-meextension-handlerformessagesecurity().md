

- MailKit
- MEExtension
-  handlerForMessageSecurity() 

Instance Method

# handlerForMessageSecurity()

Returns an object that applies security measures such as encryption and digital signatures to messages.

macOS 12.0+

``` source
@MainActor
optional func handlerForMessageSecurity() -> any MEMessageSecurityHandler
```

## Return Value

An object that encrypts, decrypts, and signs messages.

