

- App License Delivery SDK
- ALDSession
-  finalizeLicenseResponse(licenseResponse:signature:) 

Instance Method

# finalizeLicenseResponse(licenseResponse:signature:)

Returns a signed license in a byte array to send in response to a license request from iOS.

``` source
func finalizeLicenseResponse(
    licenseResponse: [UInt8],
    signature: [UInt8]? = nil
) throws -> [UInt8]
```

## Parameters 

`licenseResponse`  

The license created by generateLicenseResponse().

`signature`  

A signature for the license, signed by the signing certificate private key.

## Return Value

The signed license in a byte array.

## Mentioned in 

Licensing alternative distribution apps

## Discussion

Encode the return result to `base64` and send it as the `"license"` key in response to an iOS license request.

You can omit the `signature` argument if you include the `signingKey` argument in the ALDProvider initializer. Otherwise, pass in a signature of the license in the `signature` argument, signed by the signing certificate private key.

For more information, see Licensing alternative distribution apps.

