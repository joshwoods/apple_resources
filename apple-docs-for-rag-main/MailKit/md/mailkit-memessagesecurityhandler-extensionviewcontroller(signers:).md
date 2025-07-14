

- MailKit
- MEMessageSecurityHandler
-  extensionViewController(signers:) 

Instance Method

# extensionViewController(signers:)

Returns a view controller that displays details about a message’s digital signature.

macOS 12.0+

``` source
@MainActor
func extensionViewController(signers messageSigners: [MEMessageSigner]) -> MEExtensionViewController?
```

**Required**

## Parameters 

`messageSigners`  

An array that contains details about who signed the message.

## Return Value

A view controller that users can display to see information about a message’s digital signature.

