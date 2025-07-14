

- Security
-  CMSDecoderGetNumSigners(\_:\_:) 

Function

# CMSDecoderGetNumSigners(\_:\_:)

Obtains the number of signers of a message.

macOS 10.5+

``` source
func CMSDecoderGetNumSigners(
    _ cmsDecoder: CMSDecoder,
    _ numSignersOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsDecoder`  

The CMSDecoder reference returned by the `CMSDecoderCreate` function.

`numSignersOut`  

On return, the number of signers of the message. Zero indicates that the message was not signed.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Call the `CMSDecoderCopySignerStatus` function to determine the status of a signature.

You cannot call this function until after you have called the `CMSDecoderFinalizeMessage` function.

## See Also

### Related Documentation

func CMSDecoderCreate(UnsafeMutablePointer&lt;CMSDecoder?>) -> OSStatus

Creates a CMSDecoder reference.

func CMSDecoderFinalizeMessage(CMSDecoder) -> OSStatus

Indicates that there is no more data to decode.

