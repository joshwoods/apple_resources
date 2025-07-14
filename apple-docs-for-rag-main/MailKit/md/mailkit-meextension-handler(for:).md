

- MailKit
- MEExtension
-  handler(for:) 

Instance Method

# handler(for:)

Returns an object that participates in the composition of a mail message.

macOS 12.0+

``` source
@MainActor
optional func handler(for session: MEComposeSession) -> any MEComposeSessionHandler
```

## Parameters 

`session`  

An object that represents a mail compose window.

## Return Value

An object that participates in the composition of a mail message.

## Discussion

MailKit invokes this method for each compose window it displays.

