

- AVFoundation
- AVContentKeyResponse
-  init(authorizationTokenData:) 

Initializer

# init(authorizationTokenData:)

Creates a content key response with an authorization token.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
convenience init(authorizationTokenData: Data)
```

## Parameters 

`authorizationTokenData`  

A data value that contains the authorization token.

## See Also

### Creating New Content Key Responses

convenience init(clearKeyData: Data, initializationVector: Data?)

Creates a new key response object for key data and initialization vector sent in the clear.

convenience init(fairPlayStreamingKeyResponseData: Data)

Creates a content key response with an encrypted key response data blob when FairPlay Streaming is the key delivery method.

