

- AVFoundation
-  AVExternalContentProtectionStatus 

Enumeration

# AVExternalContentProtectionStatus

Constants that specify whether sufficient protection exists to display the content.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+

``` source
enum AVExternalContentProtectionStatus
```

## Topics

### Status values

case pending

A status that indicates content protections are pending.

case sufficient

A status that indicates sufficient protections exists for display.

case insufficient

A status that indicates insufficient protections exists for display.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### FairPlay Streaming

class AVContentKeySession

An object that creates and tracks decryption keys for media data.

protocol AVContentKeySessionDelegate

A protocol that handles content key requests.

class AVContentKey

An object that represents the content key decryptor.

class AVContentKeySpecifier

An object that uniquely identifies a content key.

class AVContentKeyRequest

An object that encapsulates information about a content decryption key request issued from a content key session object.

class AVPersistableContentKeyRequest

An object that encapsulates information about a persistable content decryption key request issued from a content key session.

class AVContentKeyResponse

An object that encapsulates information about a response to a content decryption key request.

func AVSampleBufferAttachContentKey(CMSampleBuffer, AVContentKey, NSErrorPointer) -> Bool

Attaches a content key to a sample buffer for the purpose of content decryption.

