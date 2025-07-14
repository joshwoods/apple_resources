

- AVFoundation
- AVContentKeySession
-  contentKeyRecipients 

Instance Property

# contentKeyRecipients

An array of content key recipients.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var contentKeyRecipients: [any AVContentKeyRecipient] { get }
```

## See Also

### Managing Content Key Recipients

protocol AVContentKeyRecipient

A protocol for requiring decryption keys for media data.

func addContentKeyRecipient(any AVContentKeyRecipient)

Tells the delegate that the specified recipient should have access to the decryption keys loaded with the session.

func removeContentKeyRecipient(any AVContentKeyRecipient)

Tells the delegate to remove the specified recipient.

