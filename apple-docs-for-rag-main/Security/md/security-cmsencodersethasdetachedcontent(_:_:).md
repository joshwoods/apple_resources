

- Security
-  CMSEncoderSetHasDetachedContent(\_:\_:) 

Function

# CMSEncoderSetHasDetachedContent(\_:\_:)

Specifies whether the signed data is to be separate from the message.

macOS 10.5+

``` source
func CMSEncoderSetHasDetachedContent(
    _ cmsEncoder: CMSEncoder,
    _ detachedContent: Bool
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the CMSEncoderCreate(_:) function.

`detachedContent`  

`TRUE` if the message should exclude the data to be signed. Prior to calling this function, the encoder defaults to `FALSE` for this setting, indicating that the message contains the data to be signed.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

A signed CMS message can optionally be sent separately from the signed data. Set `detachedContent` to `TRUE` to indicate that the signed data is to be kept separate from the message.

Encrypted messages, including those that are also signed, cannot use detached content.

If you do call this function, you must call it before the first call to the CMSEncoderUpdateContent(_:_:_:) function.

## See Also

### Related Documentation

func CMSEncoderGetHasDetachedContent(CMSEncoder, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Indicates whether the message is to have detached content.

func CMSEncoderUpdateContent(CMSEncoder, UnsafeRawPointer, Int) -> OSStatus

Feeds content bytes into the encoder.

func CMSEncoderCreate(UnsafeMutablePointer&lt;CMSEncoder?>) -> OSStatus

Creates a CMSEncoder reference.

func CMSDecoderSetDetachedContent(CMSDecoder, CFData) -> OSStatus

Specifies the message’s detached content, if any.

