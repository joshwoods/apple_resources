

- AVFoundation
- AVContentKeyResponse
-  init(clearKeyData:initializationVector:) 

Initializer

# init(clearKeyData:initializationVector:)

Creates a new key response object for key data and initialization vector sent in the clear.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 7.0+

``` source
convenience init(
    clearKeyData keyData: Data,
    initializationVector: Data?
)
```

## Parameters 

`keyData`  

The key used for decrypting content.

`initializationVector`  

The initialization vector used for decrypting content. This value is `nil` when the initialization vector is contained in the media to be decrypted.

## Return Value

Returns a new AVContentKeyResponse object to decrypt content.

## Discussion

Use the results of this initializer when the content key session creates a key request using the clearKey parameter. The results are then passed to the processContentKeyResponse(_:) method to supply the decrypter with key data.

## See Also

### Creating New Content Key Responses

convenience init(fairPlayStreamingKeyResponseData: Data)

Creates a content key response with an encrypted key response data blob when FairPlay Streaming is the key delivery method.

convenience init(authorizationTokenData: Data)

Creates a content key response with an authorization token.

