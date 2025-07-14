

- AVFoundation
- AVContentKeyResponse
-  init(fairPlayStreamingKeyResponseData:) 

Initializer

# init(fairPlayStreamingKeyResponseData:)

Creates a content key response with an encrypted key response data blob when FairPlay Streaming is the key delivery method.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
convenience init(fairPlayStreamingKeyResponseData keyResponseData: Data)
```

## Parameters 

`keyResponseData`  

The key data from the FairPlay Streaming key server.

## Return Value

Returns a new AVContentKeyResponse object to decrypt content.

## Discussion

Use the results of this initializer when the content key session creates a key request using the fairPlayStreaming parameter. The results are then passed to the processContentKeyResponse(_:) method to supply the decrypter with key data.

## See Also

### Creating New Content Key Responses

convenience init(clearKeyData: Data, initializationVector: Data?)

Creates a new key response object for key data and initialization vector sent in the clear.

convenience init(authorizationTokenData: Data)

Creates a content key response with an authorization token.

