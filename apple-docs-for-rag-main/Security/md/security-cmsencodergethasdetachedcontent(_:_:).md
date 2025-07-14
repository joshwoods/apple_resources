

- Security
-  CMSEncoderGetHasDetachedContent(\_:\_:) 

Function

# CMSEncoderGetHasDetachedContent(\_:\_:)

Indicates whether the message is to have detached content.

macOS 10.5+

``` source
func CMSEncoderGetHasDetachedContent(
    _ cmsEncoder: CMSEncoder,
    _ detachedContentOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the `CMSEncoderCreate` function.

`detachedContentOut`  

Returns `TRUE` if the message has detached content.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This function returns the value specified in `CMSEncoderSetHasDetachedContent` if that function has been called; otherwise it returns `FALSE`.

## See Also

### Related Documentation

func CMSEncoderSetHasDetachedContent(CMSEncoder, Bool) -> OSStatus

Specifies whether the signed data is to be separate from the message.

func CMSDecoderCreate(UnsafeMutablePointer&lt;CMSDecoder?>) -> OSStatus

Creates a CMSDecoder reference.

