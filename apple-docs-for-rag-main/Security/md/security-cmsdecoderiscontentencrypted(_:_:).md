

- Security
-  CMSDecoderIsContentEncrypted(\_:\_:) 

Function

# CMSDecoderIsContentEncrypted(\_:\_:)

Determines whether a CMS message was encrypted.

macOS 10.5+

``` source
func CMSDecoderIsContentEncrypted(
    _ cmsDecoder: CMSDecoder,
    _ isEncryptedOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsDecoder`  

The CMSDecoder reference returned by the `CMSDecoderCreate` function.

`isEncryptedOut`  

Returns `TRUE` if the message was encrypted.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Note that if the message was encrypted and the decoding succeeded (`CMSDecoderFinalizeMessage` returned `noErr`), then the message was successfully decrypted. Call CMSDecoderCopyContent(_:_:) to retrieve the decrypted content.

You cannot call this function until after you have called the `CMSDecoderFinalizeMessage` function.

## See Also

### Related Documentation

func CMSDecoderCreate(UnsafeMutablePointer&lt;CMSDecoder?>) -> OSStatus

Creates a CMSDecoder reference.

func CMSEncoderAddRecipients(CMSEncoder, CFTypeRef) -> OSStatus

Specifies a message is to be encrypted and specifies the recipients of the message.

func CMSDecoderFinalizeMessage(CMSDecoder) -> OSStatus

Indicates that there is no more data to decode.

