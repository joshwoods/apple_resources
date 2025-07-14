

- Security
-  CMSDecoderCopySignerSigningTime(\_:\_:\_:) 

Function

# CMSDecoderCopySignerSigningTime(\_:\_:\_:)

Obtains the signing time of a CMS message, if present.

macOS 10.8+

``` source
func CMSDecoderCopySignerSigningTime(
    _ cmsDecoder: CMSDecoder,
    _ signerIndex: Int,
    _ signingTime: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsDecoder`  

A CMSDecoder reference returned by the `CMSDecoderCreate` function.

`signerIndex`  

A number indicating which signer to examine. Signer index numbers start with 0. Use the CMSDecoderGetNumSigners(_:_:) function to determine the total number of signers for a message.

`signingTime`  

The address of an absolute time value where the result should be stored.

## Return Value

A result code. See Security Framework Result Codes. Typically, this function returns errSecParam if the CMS message was not signed or if `signerIndex` is out of bounds.

## Discussion

The timestamp is an unauthenticated time, although it is part of the signed attributes of the message.

You must call CMSDecoderFinalizeMessage(_:) before you call this function.

