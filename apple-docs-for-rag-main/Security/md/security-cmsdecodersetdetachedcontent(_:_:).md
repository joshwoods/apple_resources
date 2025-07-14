

- Security
-  CMSDecoderSetDetachedContent(\_:\_:) 

Function

# CMSDecoderSetDetachedContent(\_:\_:)

Specifies the message’s detached content, if any.

macOS 10.5+

``` source
func CMSDecoderSetDetachedContent(
    _ cmsDecoder: CMSDecoder,
    _ detachedContent: CFData
) -> OSStatus
```

## Parameters 

`cmsDecoder`  

The CMSDecoder reference returned by the `CMSDecoderCreate` function.

`detachedContent`  

A reference to the message’s detached content.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

The data of a signed CMS message can optionally be sent separately from the message. If the message’s content is detached from the message, you must call this function to tell the decoder where to find the message content.

Encrypted messages, including those that are also signed, cannot use detached content.

You can call this function either before or after decoding the message (by calling the `CMSDecoderUpdateMessage` and `CMSDecoderFinalizeMessage` functions). If a signed message has detached content, however, you must call this function before you can use the `CMSDecoderCopySignerStatus` function to ascertain the signature status.

## See Also

### Related Documentation

func CMSEncoderSetHasDetachedContent(CMSEncoder, Bool) -> OSStatus

Specifies whether the signed data is to be separate from the message.

func CMSDecoderCreate(UnsafeMutablePointer&lt;CMSDecoder?>) -> OSStatus

Creates a CMSDecoder reference.

func CMSDecoderCopySignerStatus(CMSDecoder, Int, CFTypeRef, Bool, UnsafeMutablePointer&lt;CMSSignerStatus>?, UnsafeMutablePointer&lt;SecTrust?>?, UnsafeMutablePointer&lt;OSStatus>?) -> OSStatus

Obtains the status of a CMS message’s signature.

