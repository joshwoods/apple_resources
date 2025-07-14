

- AVFoundation
- AVContentKeySessionDelegate
-  contentKeySession(\_:contentKeyRequest:didFailWithError:) 

Instance Method

# contentKeySession(\_:contentKeyRequest:didFailWithError:)

Tells the receiver that the content key request failed.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
optional func contentKeySession(
    _ session: AVContentKeySession,
    contentKeyRequest keyRequest: AVContentKeyRequest,
    didFailWithError err: any Error
)
```

## Parameters 

`session`  

The content key session that initiated the content key request.

`keyRequest`  

The content key request that failed.

`err`  

An instance of NSError that describes the failure that occurred.

## See Also

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

func contentKeySession(AVContentKeySession, contentKeyRequestDidSucceed: AVContentKeyRequest)

Tells the content key session that the response to a content key requeset was successfully processed.

func contentKeySessionDidGenerateExpiredSessionReport(AVContentKeySession)

Notifies the sender that an expired session report has been generated.

