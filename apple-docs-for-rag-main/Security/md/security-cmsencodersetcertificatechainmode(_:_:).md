

- Security
-  CMSEncoderSetCertificateChainMode(\_:\_:) 

Function

# CMSEncoderSetCertificateChainMode(\_:\_:)

Specifies which certificates to include in a signed CMS message.

macOS 10.5+

``` source
func CMSEncoderSetCertificateChainMode(
    _ cmsEncoder: CMSEncoder,
    _ chainMode: CMSCertificateChainMode
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the `CMSEncoderCreate` function.

`chainMode`  

A constant that indicates which certificate or certificates to include in the message. See CMSCertificateChainMode.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This function is used only for signed messages and is optional. If you don’t call this function, the default, `kCMSCertificateChain`, is used. In this case the message includes the signer certificate plus all certificates needed to verify the signer certificate, up to but not including the root certificate.

If you do call this function, you must call it before the first call to the `CMSEncoderUpdateContent` function.

## See Also

### Related Documentation

func CMSEncoderUpdateContent(CMSEncoder, UnsafeRawPointer, Int) -> OSStatus

Feeds content bytes into the encoder.

func CMSEncoderGetCertificateChainMode(CMSEncoder, UnsafeMutablePointer&lt;CMSCertificateChainMode>) -> OSStatus

Obtains a constant that indicates which certificates are to be included in a signed CMS message.

func CMSEncoderCreate(UnsafeMutablePointer&lt;CMSEncoder?>) -> OSStatus

Creates a CMSEncoder reference.

