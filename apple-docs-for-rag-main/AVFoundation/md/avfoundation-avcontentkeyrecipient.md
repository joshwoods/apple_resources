

- AVFoundation
-  AVContentKeyRecipient 

Protocol

# AVContentKeyRecipient

A protocol for requiring decryption keys for media data.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
protocol AVContentKeyRecipient
```

## Topics

### Verifying Decryption Key Requirements

var mayRequireContentKeysForMediaDataProcessing: Bool

A Boolean value that indicates whether the recipient requires decryption keys for media data to enable processing.

**Required**

func contentKeySession(AVContentKeySession, didProvide: AVContentKey)

Tells the recipient that a content key is available.

## Relationships

### Conforming Types

- AVFragmentedAsset
- AVURLAsset

## See Also

### Managing Content Key Recipients

var contentKeyRecipients: [any AVContentKeyRecipient]

An array of content key recipients.

func addContentKeyRecipient(any AVContentKeyRecipient)

Tells the delegate that the specified recipient should have access to the decryption keys loaded with the session.

func removeContentKeyRecipient(any AVContentKeyRecipient)

Tells the delegate to remove the specified recipient.

