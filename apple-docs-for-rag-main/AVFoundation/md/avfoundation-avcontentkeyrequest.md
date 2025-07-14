

- AVFoundation
-  AVContentKeyRequest 

Class

# AVContentKeyRequest

An object that encapsulates information about a content decryption key request issued from a content key session object.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
class AVContentKeyRequest
```

## Topics

### Getting Content Key Request Data

func makeStreamingContentKeyRequestData(forApp: Data, contentIdentifier: Data?, options: [String : Any]?, completionHandler: (Data?, (any Error)?) -> Void)

Obtains encrypted key request data for a specific combination of app and content.

let AVContentKeyRequestProtocolVersionsKey: String

A key that specifies the versions of the content protection protocol supported by the application.

let AVContentKeyRequestRequiresValidationDataInSecureTokenKey: String

A key that requires the secure token to have extended validation data.

### Responding to the Content Key Request

func respondByRequestingPersistableContentKeyRequest()

Tells the receiver that the app requires a persistable content key request object for processing.

Deprecated

func processContentKeyResponse(AVContentKeyResponse)

Sends the specified content key response to the receiver for processing.

func processContentKeyResponseError(any Error)

Tells the receiver that the app was unable to obtain a content key response.

func respondByRequestingPersistableContentKeyRequest()

Tells the receiver that the app requires a persistable content key request object for processing.

Deprecated

### Getting Content Key Request Properties

var identifier: (any Sendable)?

The identifier for the content key.

var canProvidePersistableContentKey: Bool

The content key request used to create a persistable content key or respond to a previous request with a persistable content key.

var error: (any Error)?

The error description for a failed key request.

var initializationData: Data?

The data used to obtain a key response.

var renewsExpiringResponseData: Bool

A Boolean value that indicates whether the content key request renews previously provided response data.

var status: AVContentKeyRequest.Status

The current state of the content key request.

enum Status

The status for a content key request.

### Inspecting a Request

var contentKey: AVContentKey?

The generated content key.

var contentKeySpecifier: AVContentKeySpecifier

The requested content key specifier.

var options: [String : any Sendable]

A dictionary of options used to initialize key loading.

struct RetryReason

The reason for asking the client to retry a content key request.

### Instance Methods

func respondByRequestingPersistableContentKeyRequestAndReturnError() throws

Tells the receiver that the app requires a persistable content key request object for processing.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVPersistableContentKeyRequest

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

class AVPersistableContentKeyRequest

An object that encapsulates information about a persistable content decryption key request issued from a content key session.

class AVContentKeyResponse

An object that encapsulates information about a response to a content decryption key request.

enum AVExternalContentProtectionStatus

Constants that specify whether sufficient protection exists to display the content.

func AVSampleBufferAttachContentKey(CMSampleBuffer, AVContentKey, NSErrorPointer) -> Bool

Attaches a content key to a sample buffer for the purpose of content decryption.

