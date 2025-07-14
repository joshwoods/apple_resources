

- Security
-  CMSDecoderCopyDetachedContent(\_:\_:) 

Function

# CMSDecoderCopyDetachedContent(\_:\_:)

Obtains the detached content specified with the `CMSDecoderSetDetachedContent` function.

macOS 10.5+

``` source
func CMSDecoderCopyDetachedContent(
    _ cmsDecoder: CMSDecoder,
    _ detachedContentOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsDecoder`  

The CMSDecoder reference returned by the `CMSDecoderCreate` function.

`detachedContentOut`  

On return, points to the data reference specified by an earlier call to the `CMSDecoderSetDetachedContent` function. Returns a NULL data reference if no detached content has been specified. You must use the `CFRelease` function to free this reference when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## See Also

### Related Documentation

func CMSDecoderCreate(UnsafeMutablePointer&lt;CMSDecoder?>) -> OSStatus

Creates a CMSDecoder reference.

