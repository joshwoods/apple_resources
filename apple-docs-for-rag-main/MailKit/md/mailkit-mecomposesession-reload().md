

- MailKit
- MEComposeSession
-  reload() 

Instance Method

# reload()

Refreshes the compose session with the extension’s new information.

macOS 12.0+

``` source
func reload()
```

## Discussion

Call this method from your extension to regenerate address annotations to replace existing annotations for the session. In response, MailKit invokes annotateAddressesForSession(_:completion:) for all addresses in the To, Cc, and Bcc fields.

## See Also

### Managing Compose Sessions

var sessionID: UUID

A unique identifier for the session.

