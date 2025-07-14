

- AVFoundation
- AVContentKeySession
-  removeContentKeyRecipient(\_:) 

Instance Method

# removeContentKeyRecipient(\_:)

Tells the delegate to remove the specified recipient.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func removeContentKeyRecipient(_ recipient: any AVContentKeyRecipient)
```

## Parameters 

`recipient`  

The content key recipient to remove.

## See Also

### Managing Content Key Recipients

var contentKeyRecipients: [any AVContentKeyRecipient]

An array of content key recipients.

protocol AVContentKeyRecipient

A protocol for requiring decryption keys for media data.

func addContentKeyRecipient(any AVContentKeyRecipient)

Tells the delegate that the specified recipient should have access to the decryption keys loaded with the session.

