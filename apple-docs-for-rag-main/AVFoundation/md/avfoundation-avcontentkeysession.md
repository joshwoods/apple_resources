

- AVFoundation
-  AVContentKeySession 

Class

# AVContentKeySession

An object that creates and tracks decryption keys for media data.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
class AVContentKeySession
```

## Topics

### Creating a Session

convenience init(keySystem: AVContentKeySystem)

Creates a content key session to manage a collection of content decryption keys.

convenience init(keySystem: AVContentKeySystem, storageDirectoryAt: URL)

Creates a content key session to manage a collection of content decryption keys; points to a directory that stores abnormal session termination reports.

### Inspecting the Session

var keySystem: AVContentKeySystem

The type of key system used to retrieve keys.

struct AVContentKeySystem

A key-delivery method for a content key session.

var storageURL: URL?

A URL that points to a writable storage directory.

### Managing the Delegate Object

func setDelegate((any AVContentKeySessionDelegate)?, queue: dispatch_queue_t?)

Sets the session’s delegate object and the dispatch queue on which to call the delegate’s methods.

var delegate: (any AVContentKeySessionDelegate)?

The content key session’s delegate object.

var delegateQueue: dispatch_queue_t?

The dispatch queue the session uses to invoke delegate callbacks.

### Managing Content Key Recipients

var contentKeyRecipients: [any AVContentKeyRecipient]

An array of content key recipients.

protocol AVContentKeyRecipient

A protocol for requiring decryption keys for media data.

func addContentKeyRecipient(any AVContentKeyRecipient)

Tells the delegate that the specified recipient should have access to the decryption keys loaded with the session.

func removeContentKeyRecipient(any AVContentKeyRecipient)

Tells the delegate to remove the specified recipient.

### Processing Requests

func processContentKeyRequest(withIdentifier: (any Sendable)?, initializationData: Data?, options: [String : any Sendable]?)

Tells the delegate to start loading the content decryption key with the specified identifier and initialization data.

### Managing Expiration

func expire()

Tells the delegate that the session expired as the result of normal, intentional processes.

func makeSecureTokenForExpirationDate(ofPersistableContentKey: Data, completionHandler: (Data?, (any Error)?) -> Void)

Creates a secure server playback context that the client sends to the key server to get an expiration date for the given persistable content key data.

func renewExpiringResponseData(for: AVContentKeyRequest)

Tells the delegate that previously provided response data for a content key request is about to expire.

var contentProtectionSessionIdentifier: Data?

The identifier for the current content protection session.

### Invalidating Content Keys

func invalidatePersistableContentKey(Data, options: [AVContentKeySessionServerPlaybackContextOption : Any]?, completionHandler: (Data?, (any Error)?) -> Void)

Invalidates the persistable content key and creates a secure server playback context (SPC) to verify the outcome of an invalidation request.

func invalidateAllPersistableContentKeys(forApp: Data, options: [AVContentKeySessionServerPlaybackContextOption : Any]?, completionHandler: (Data?, (any Error)?) -> Void)

Invalidates all of an app’s persistable content keys and creates a secure server playback context (SPC) to verify the outcome of an invalidation request.

struct AVContentKeySessionServerPlaybackContextOption

Options for specifying additional information for generating server playback context (SPC).

### Handling Expired Session Reports

class func pendingExpiredSessionReports(withAppIdentifier: Data, storageDirectoryAt: URL) -> [Data]

Returns the expired session reports for content key sessions created with the specified app identifier.

class func removePendingExpiredSessionReports([Data], withAppIdentifier: Data, storageDirectoryAt: URL)

Removes expired session reports from storage.

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

enum AVExternalContentProtectionStatus

Constants that specify whether sufficient protection exists to display the content.

func AVSampleBufferAttachContentKey(CMSampleBuffer, AVContentKey, NSErrorPointer) -> Bool

Attaches a content key to a sample buffer for the purpose of content decryption.

