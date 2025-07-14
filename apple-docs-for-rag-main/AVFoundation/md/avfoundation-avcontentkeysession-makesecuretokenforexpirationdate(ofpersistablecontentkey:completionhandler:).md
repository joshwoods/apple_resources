

- AVFoundation
- AVContentKeySession
-  makeSecureTokenForExpirationDate(ofPersistableContentKey:completionHandler:) 

Instance Method

# makeSecureTokenForExpirationDate(ofPersistableContentKey:completionHandler:)

Creates a secure server playback context that the client sends to the key server to get an expiration date for the given persistable content key data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+tvOS 17.0+visionOS 1.0+watchOS 7.0+

``` source
func makeSecureTokenForExpirationDate(
    ofPersistableContentKey persistableContentKeyData: Data,
    completionHandler handler: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func makeSecureTokenForExpirationDate(ofPersistableContentKey persistableContentKeyData: Data) async throws -> Data
```

## Parameters 

`persistableContentKeyData`  

The previously created persistable content key data.

`handler`  

A block called after the secure token is ready.

secureTokenData  
The new secure token.

error  
A parameter that holds the error object that explains the error. If no error occurred, the value of this parameter is `nil`.

## See Also

### Managing Expiration

func expire()

Tells the delegate that the session expired as the result of normal, intentional processes.

func renewExpiringResponseData(for: AVContentKeyRequest)

Tells the delegate that previously provided response data for a content key request is about to expire.

var contentProtectionSessionIdentifier: Data?

The identifier for the current content protection session.

