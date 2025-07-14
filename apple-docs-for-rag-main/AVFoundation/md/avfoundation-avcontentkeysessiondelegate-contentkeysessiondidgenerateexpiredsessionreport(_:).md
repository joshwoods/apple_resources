

- AVFoundation
- AVContentKeySessionDelegate
-  contentKeySessionDidGenerateExpiredSessionReport(\_:) 

Instance Method

# contentKeySessionDidGenerateExpiredSessionReport(\_:)

Notifies the sender that an expired session report has been generated.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 7.0+

``` source
optional func contentKeySessionDidGenerateExpiredSessionReport(_ session: AVContentKeySession)
```

## Parameters 

`session`  

The AVContentKeySession object that recorded the generation of an expired session report.

## Discussion

This method is invoked when an expired session report is added to the storageURL property.

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

func contentKeySession(AVContentKeySession, contentKeyRequest: AVContentKeyRequest, didFailWithError: any Error)

Tells the receiver that the content key request failed.

func contentKeySession(AVContentKeySession, contentKeyRequestDidSucceed: AVContentKeyRequest)

Tells the content key session that the response to a content key requeset was successfully processed.

