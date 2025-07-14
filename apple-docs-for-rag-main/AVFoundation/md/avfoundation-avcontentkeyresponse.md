

- AVFoundation
-  AVContentKeyResponse 

Class

# AVContentKeyResponse

An object that encapsulates information about a response to a content decryption key request.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
class AVContentKeyResponse
```

## Topics

### Creating New Content Key Responses

convenience init(clearKeyData: Data, initializationVector: Data?)

Creates a new key response object for key data and initialization vector sent in the clear.

convenience init(fairPlayStreamingKeyResponseData: Data)

Creates a content key response with an encrypted key response data blob when FairPlay Streaming is the key delivery method.

convenience init(authorizationTokenData: Data)

Creates a content key response with an authorization token.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
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

enum AVExternalContentProtectionStatus

Constants that specify whether sufficient protection exists to display the content.

func AVSampleBufferAttachContentKey(CMSampleBuffer, AVContentKey, NSErrorPointer) -> Bool

Attaches a content key to a sample buffer for the purpose of content decryption.

