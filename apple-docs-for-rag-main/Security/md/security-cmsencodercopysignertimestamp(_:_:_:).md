

- Security
-  CMSEncoderCopySignerTimestamp(\_:\_:\_:) 

Function

# CMSEncoderCopySignerTimestamp(\_:\_:\_:)

Returns the timestamp of a signer of a CMS message, if present.

macOS 10.8+

``` source
func CMSEncoderCopySignerTimestamp(
    _ cmsEncoder: CMSEncoder,
    _ signerIndex: Int,
    _ timestamp: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

A CMSEncoder reference returned by the `CMSEncoderCreate` function.

`signerIndex`  

A number indicating which signer to examine. Signer index numbers start with 0. Use the CMSDecoderGetNumSigners(_:_:) function to determine the total number of signers for a message.

`timestamp`  

The address of an absolute time value where the result should be stored.

## Return Value

A result code. See Security Framework Result Codes. Typically, this function returns errSecParam if the CMS message was not signed or if `signerIndex` is out of bounds.

## Discussion

This timestamp is an authenticated timestamp provided by a time stamping authority.

You must call CMSDecoderFinalizeMessage(_:) before you call this function.

