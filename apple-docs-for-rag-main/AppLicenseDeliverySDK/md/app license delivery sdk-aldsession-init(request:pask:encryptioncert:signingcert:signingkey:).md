

- App License Delivery SDK
- ALDSession
-  init(request:PASK:encryptionCert:signingCert:signingKey:) 

Initializer

# init(request:PASK:encryptionCert:signingCert:signingKey:)

Initialize a ALDSession with a license request. Call generateLicense() to create a license.

``` source
init(
    request: [UInt8],
    PASK: [UInt8],
    encryptionCert: [UInt8],
    signingCert: [UInt8],
    signingKey: [UInt8]? = nil
) throws
```

## Parameters 

`request`  

Opaque request bytes sent by the client

`PASK`  

The server side secret provided to the provider

`encryptionCert`  

The ALD provider encryption cert

`signingCert`  

The ALD provider signing cert

`signingKey`  

The ALD provider signing key in DER encoded format. When provided, one can use finalizeLicenseResponse() to automarically sign the payload. If this key is not provided, then one must sign each license payload out of band and add it to the license response.

