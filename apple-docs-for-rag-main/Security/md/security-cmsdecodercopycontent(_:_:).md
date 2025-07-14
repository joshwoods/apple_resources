

- Security
-  CMSDecoderCopyContent(\_:\_:) 

Function

# CMSDecoderCopyContent(\_:\_:)

Obtains the message content, if any.

macOS 10.5+

``` source
func CMSDecoderCopyContent(
    _ cmsDecoder: CMSDecoder,
    _ contentOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsDecoder`  

The CMSDecoder reference returned by the `CMSDecoderCreate` function.

`contentOut`  

On return, points to the message’s content. Returns `NULL` if the content is detached. You must use the `CFRelease` function to free this reference when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

If the message has detached content, you are responsible for retrieving the content. In that case, you use the CMSDecoderSetDetachedContent(_:_:) function to tell the decoder the location of the content.

You cannot call this function until after you have called the `CMSDecoderFinalizeMessage` function.

## See Also

### Related Documentation

func CMSEncoderSetHasDetachedContent(CMSEncoder, Bool) -> OSStatus

Specifies whether the signed data is to be separate from the message.

func CMSDecoderSetDetachedContent(CMSDecoder, CFData) -> OSStatus

Specifies the message’s detached content, if any.

func CMSDecoderCreate(UnsafeMutablePointer&lt;CMSDecoder?>) -> OSStatus

Creates a CMSDecoder reference.

func CMSDecoderFinalizeMessage(CMSDecoder) -> OSStatus

Indicates that there is no more data to decode.

