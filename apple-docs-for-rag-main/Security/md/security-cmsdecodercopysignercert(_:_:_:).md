

- Security
-  CMSDecoderCopySignerCert(\_:\_:\_:) 

Function

# CMSDecoderCopySignerCert(\_:\_:\_:)

Obtains the certificate of the specified signer of a CMS message.

macOS 10.5+

``` source
func CMSDecoderCopySignerCert(
    _ cmsDecoder: CMSDecoder,
    _ signerIndex: Int,
    _ signerCertOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsDecoder`  

The CMSDecoder reference returned by the `CMSDecoderCreate` function.

`signerIndex`  

A number indicating which signer’s email address to return. Signer index numbers start with 0. Use the CMSDecoderGetNumSigners(_:_:) function to determine the total number of signers for a message.

`signerCertOut`  

On return, points to the certificate of the specified signer.

## Return Value

A result code. See Security Framework Result Codes. Returns errSecParam if the CMS message was not signed or if `signerIndex` is greater than the number of signers of the message minus one (signerIndex \> (numSigners – 1)).

## Discussion

You cannot call this function until after you have called the CMSDecoderFinalizeMessage(_:) function.

## See Also

### Related Documentation

func CMSDecoderCreate(UnsafeMutablePointer&lt;CMSDecoder?>) -> OSStatus

Creates a CMSDecoder reference.

func CMSDecoderFinalizeMessage(CMSDecoder) -> OSStatus

Indicates that there is no more data to decode.

