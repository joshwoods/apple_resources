

- AVFoundation
- AVContentKeySession
-  expire() 

Instance Method

# expire()

Tells the delegate that the session expired as the result of normal, intentional processes.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
func expire()
```

## See Also

### Managing Expiration

func makeSecureTokenForExpirationDate(ofPersistableContentKey: Data, completionHandler: (Data?, (any Error)?) -> Void)

Creates a secure server playback context that the client sends to the key server to get an expiration date for the given persistable content key data.

func renewExpiringResponseData(for: AVContentKeyRequest)

Tells the delegate that previously provided response data for a content key request is about to expire.

var contentProtectionSessionIdentifier: Data?

The identifier for the current content protection session.

