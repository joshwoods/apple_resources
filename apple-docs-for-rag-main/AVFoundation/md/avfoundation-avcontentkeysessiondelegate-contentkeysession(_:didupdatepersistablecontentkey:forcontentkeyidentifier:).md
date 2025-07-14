

- AVFoundation
- AVContentKeySessionDelegate
-  contentKeySession(\_:didUpdatePersistableContentKey:forContentKeyIdentifier:) 

Instance Method

# contentKeySession(\_:didUpdatePersistableContentKey:forContentKeyIdentifier:)

Provides the receiver with an updated persistable content key for a specific key request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+tvOS 17.0+visionOS 1.0+watchOS 7.0+

``` source
optional func contentKeySession(
    _ session: AVContentKeySession,
    didUpdatePersistableContentKey persistableContentKey: Data,
    forContentKeyIdentifier keyIdentifier: Any
)
```

## Parameters 

`session`  

The content key session that is providing the updated persistable content key.

`persistableContentKey`  

The updated persistent content key data. This data can be stored offline and used to answer future content key requests with the matching key identifier.

`keyIdentifier`  

A container- and protocol-specific identifier for the updated persistent content key.

## Discussion

If the content key session provides updated persistable content key data, previous key data is no longer valid and cannot be used to answer future loading requests.

## See Also

### Updating and Retrying Content Key Requests

func contentKeySession(AVContentKeySession, didProvide: [AVContentKeyRequest], forInitializationData: Data?)

func contentKeySession(AVContentKeySession, externalProtectionStatusDidChangeFor: AVContentKey)

Tells the delegate when external protection state has changed.

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

