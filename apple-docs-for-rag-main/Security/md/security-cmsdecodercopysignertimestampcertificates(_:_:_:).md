

- Security
-  CMSDecoderCopySignerTimestampCertificates(\_:\_:\_:) 

Function

# CMSDecoderCopySignerTimestampCertificates(\_:\_:\_:)

Returns an array containing the certificates from a timestamp response.

macOS 10.8+

``` source
func CMSDecoderCopySignerTimestampCertificates(
    _ cmsDecoder: CMSDecoder,
    _ signerIndex: Int,
    _ certificateRefs: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsDecoder`  

A CMSDecoder reference returned by the `CMSDecoderCreate` function.

`signerIndex`  

A number indicating which signer to examine. Signer index numbers start with 0. Use the CMSDecoderGetNumSigners(_:_:) function to determine the total number of signers for a message.

`certificateRefs`  

The address of a Core Foundation array reference where the resulting array should be stored.

## Return Value

A result code. See Security Framework Result Codes. Typically, this function returns errSecParam if the CMS message was not signed or `signerIndex` is out of bounds, and returns errSecItemNotFound if no certificates were found.

## Discussion

The signature must contain an authenticated timestamp provided by a time stamping authority. Elements of the returned array are of type `SecCertificateRef`. The caller is responsible for releasing the returned array by calling `CFRelease`.

You must call CMSDecoderFinalizeMessage(_:) before you call this function.

