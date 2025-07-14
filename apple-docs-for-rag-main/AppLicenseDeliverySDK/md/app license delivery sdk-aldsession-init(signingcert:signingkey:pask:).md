

- App License Delivery SDK
- ALDSession
-  init(signingCert:signingKey:PASK:) 

Initializer

# init(signingCert:signingKey:PASK:)

Initialize a static ALDSession without a request. This should only be used when an offline generation of a static license is desired. A static license is a minimal license that is only used to install apps on the device and is not meant to enforce marketplace defined rights. Only generateStaticLicense() should be invoked to generate licenses in this case.

``` source
init(
    signingCert: [UInt8],
    signingKey: [UInt8]? = nil,
    PASK: [UInt8]
) throws
```

## Parameters 

`signingCert`  

The ALD provider signing cert

`signingKey`  

The ALD provider signing key in DER encoded format. When provided, one can use finalizeLicenseResponse() to automarically sign the payload. If this key is not provided, then one must sign each license payload out of band and add it to the license response.

`PASK`  

The server side secret provided to the provider

