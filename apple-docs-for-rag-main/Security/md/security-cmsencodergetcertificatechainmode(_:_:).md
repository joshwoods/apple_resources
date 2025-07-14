

- Security
-  CMSEncoderGetCertificateChainMode(\_:\_:) 

Function

# CMSEncoderGetCertificateChainMode(\_:\_:)

Obtains a constant that indicates which certificates are to be included in a signed CMS message.

macOS 10.5+

``` source
func CMSEncoderGetCertificateChainMode(
    _ cmsEncoder: CMSEncoder,
    _ chainModeOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the `CMSEncoderCreate` function.

`chainModeOut`  

On return, a constant that indicates which certificate or certificates are to be included in the message. See CMSCertificateChainMode.

## Return Value

A result code. See Security Framework Result Codes.

## See Also

### Related Documentation

func CMSEncoderCreate(UnsafeMutablePointer&lt;CMSEncoder?>) -> OSStatus

Creates a CMSEncoder reference.

