

- AVFoundation
-  AVContentKeySessionDelegate 

Protocol

# AVContentKeySessionDelegate

A protocol that handles content key requests.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
protocol AVContentKeySessionDelegate : NSObjectProtocol, Sendable
```

## Topics

### Providing New Content Key Requests

func contentKeySession(AVContentKeySession, didProvide: AVContentKeyRequest)

Provides the receiver with a new content key request object.

**Required**

func contentKeySession(AVContentKeySession, didProvideRenewingContentKeyRequest: AVContentKeyRequest)

Provides the receiver with a new content key request object for the renewal of an existing content key.

func contentKeySession(AVContentKeySession, didProvide: AVPersistableContentKeyRequest)

Provides the receiver with a new content key request object to process a persistable content key.

### Updating and Retrying Content Key Requests

func contentKeySession(AVContentKeySession, didProvide: [AVContentKeyRequest], forInitializationData: Data?)

func contentKeySession(AVContentKeySession, externalProtectionStatusDidChangeFor: AVContentKey)

Tells the delegate when external protection state has changed.

func contentKeySession(AVContentKeySession, didUpdatePersistableContentKey: Data, forContentKeyIdentifier: Any)

Provides the receiver with an updated persistable content key for a specific key request.

func contentKeySession(AVContentKeySession, shouldRetry: AVContentKeyRequest, reason: AVContentKeyRequest.RetryReason) -> Bool

Provides the receiver with a content key request object to retry.

struct RetryReason

The reason for asking the client to retry a content key request.

func contentKeySessionContentProtectionSessionIdentifierDidChange(AVContentKeySession)

Tells the receiver the content protection session identifier changed.

func contentKeySession(AVContentKeySession, contentKeyRequest: AVContentKeyRequest, didFailWithError: any Error)

Tells the receiver that the content key request failed.

func contentKeySession(AVContentKeySession, contentKeyRequestDidSucceed: AVContentKeyRequest)

Tells the content key session that the response to a content key requeset was successfully processed.

func contentKeySessionDidGenerateExpiredSessionReport(AVContentKeySession)

Notifies the sender that an expired session report has been generated.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

## See Also

### FairPlay Streaming

class AVContentKeySession

An object that creates and tracks decryption keys for media data.

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

enum AVExternalContentProtectionStatus

Constants that specify whether sufficient protection exists to display the content.

func AVSampleBufferAttachContentKey(CMSampleBuffer, AVContentKey, NSErrorPointer) -> Bool

Attaches a content key to a sample buffer for the purpose of content decryption.

