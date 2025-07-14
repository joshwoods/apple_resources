

- AVFoundation
- AVContentKeySession
-  addContentKeyRecipient(\_:) 

Instance Method

# addContentKeyRecipient(\_:)

Tells the delegate that the specified recipient should have access to the decryption keys loaded with the session.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func addContentKeyRecipient(_ recipient: any AVContentKeyRecipient)
```

## Parameters 

`recipient`  

The content key recipient to use for the session.

## Discussion

Don’t add a recipient to a session that has expired or had already begun to process media data.

## See Also

### Managing Content Key Recipients

var contentKeyRecipients: [any AVContentKeyRecipient]

An array of content key recipients.

protocol AVContentKeyRecipient

A protocol for requiring decryption keys for media data.

func removeContentKeyRecipient(any AVContentKeyRecipient)

Tells the delegate to remove the specified recipient.

