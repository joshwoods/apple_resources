

- AVFoundation
- AVContentKeySessionDelegate
-  contentKeySession(\_:shouldRetry:reason:) 

Instance Method

# contentKeySession(\_:shouldRetry:reason:)

Provides the receiver with a content key request object to retry.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
optional func contentKeySession(
    _ session: AVContentKeySession,
    shouldRetry keyRequest: AVContentKeyRequest,
    reason retryReason: AVContentKeyRequest.RetryReason
) -> Bool
```

## Parameters 

`session`  

The content key session that is providing the content key request.

`keyRequest`  

The key request to be retried.

`retryReason`  

The reason for the retry request.

## See Also

### Updating and Retrying Content Key Requests

func contentKeySession(AVContentKeySession, didProvide: [AVContentKeyRequest], forInitializationData: Data?)

func contentKeySession(AVContentKeySession, externalProtectionStatusDidChangeFor: AVContentKey)

Tells the delegate when external protection state has changed.

func contentKeySession(AVContentKeySession, didUpdatePersistableContentKey: Data, forContentKeyIdentifier: Any)

Provides the receiver with an updated persistable content key for a specific key request.

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

