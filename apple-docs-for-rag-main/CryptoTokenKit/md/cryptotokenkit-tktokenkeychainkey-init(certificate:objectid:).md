

- CryptoTokenKit
- TKTokenKeychainKey
-  init(certificate:objectID:) 

Initializer

# init(certificate:objectID:)

Initializes a token keychain key with data from the specified certificate reference and a given object ID.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init?(
    certificate certificateRef: SecCertificate?,
    objectID: TKToken.ObjectID
)
```

## Parameters 

`certificateRef`  

The certificate reference.

You can create a `SecCertificateRef` value from a data object using the `SecCertificateCreateWithData` function.

`objectID`  

The object ID.

## Return Value

A new token keychain certificate.

## Discussion

This is the designated initializer.

