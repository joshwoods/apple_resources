

- PassKit (Apple Pay and Wallet)
- PKIdentityDocument
-  encryptedData 

Instance Property

# encryptedData

An encrypted data object that contains the document information and metadata to associate with a request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
var encryptedData: Data { get }
```

## Mentioned in 

Requesting identity data from a Wallet pass

## Discussion

The system encrypts this property to the public key with the developer portal for the calling app. You need to send this data to the server holding the corresponding private key for decryption.

