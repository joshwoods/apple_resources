

- App License Delivery SDK
- ALDProvider
-  init(encryptionCert:signingCert:PASK:signingKey:) 

Initializer

# init(encryptionCert:signingCert:PASK:signingKey:)

Initializes a provider with the marketplace’s App License Delivery assets and their unique signing key.

``` source
init(
    encryptionCert: [UInt8],
    signingCert: [UInt8],
    PASK: [UInt8],
    signingKey: [UInt8]? = nil
)
```

## Parameters 

`encryptionCert`  

Apple issued encryption certificate in bytes.

`signingCert`  

Apple issued signing certificate in bytes.

`PASK`  

Apple provided secret blob.

`signingKey`  

Private key corresponding to the `signingCert` in `.DER` format with `ANS.1` encoding. This parameter is optional if you choose to sign the license response manually.

## Mentioned in 

Licensing alternative distribution apps

## Discussion

For an example that uses a provider, see Licensing alternative distribution apps.

