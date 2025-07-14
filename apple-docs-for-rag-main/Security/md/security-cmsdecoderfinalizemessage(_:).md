

- Security
-  CMSDecoderFinalizeMessage(\_:) 

Function

# CMSDecoderFinalizeMessage(\_:)

Indicates that there is no more data to decode.

macOS 10.5+

``` source
func CMSDecoderFinalizeMessage(_ cmsDecoder: CMSDecoder) -> OSStatus
```

## Parameters 

`cmsDecoder`  

The CMSDecoder reference returned by the `CMSDecoderCreate` function.

## Return Value

A result code. See Security Framework Result Codes. Returns errSecUnknownFormat upon detection of an improperly formatted CMS message.

## Discussion

When you call this function, the decoder finishes decoding the message. If the message was encrypted and this function returns a result code of `noErr`, the message was successfully decrypted. Call the CMSDecoderCopyContent(_:_:) function to retrieve the message content. Call the CMSDecoderGetNumSigners(_:_:) function to find out if the message was signed and, if so, how many signers there were.

## See Also

### Related Documentation

func CMSDecoderGetNumSigners(CMSDecoder, UnsafeMutablePointer&lt;Int>) -> OSStatus

Obtains the number of signers of a message.

func CMSDecoderCreate(UnsafeMutablePointer&lt;CMSDecoder?>) -> OSStatus

Creates a CMSDecoder reference.

func CMSDecoderCopyContent(CMSDecoder, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Obtains the message content, if any.

