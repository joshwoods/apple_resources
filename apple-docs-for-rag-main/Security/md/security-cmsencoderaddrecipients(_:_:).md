

- Security
-  CMSEncoderAddRecipients(\_:\_:) 

Function

# CMSEncoderAddRecipients(\_:\_:)

Specifies a message is to be encrypted and specifies the recipients of the message.

macOS 10.5+

``` source
func CMSEncoderAddRecipients(
    _ cmsEncoder: CMSEncoder,
    _ recipientOrArray: CFTypeRef
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the `CMSEncoderCreate` function.

`recipientOrArray`  

Either a single certificate containing a public encryption key for one message recipient, specified as a certificate object (type SecCertificate), or a set of certificates specified as a CFArray of certificate objects.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Your keychain must contain a certificate that supports encryption for each recipient. You can call this function more than once for the same message.

You can both sign and encrypt the same message; however, you cannot call both this function and the CMSEncoderSetHasDetachedContent(_:_:) function for the same message.

If you do call this function, you must call it before the first call to the CMSEncoderUpdateContent(_:_:_:) function.

## See Also

### Related Documentation

func CMSEncoderUpdateContent(CMSEncoder, UnsafeRawPointer, Int) -> OSStatus

Feeds content bytes into the encoder.

func CMSEncoderCreate(UnsafeMutablePointer&lt;CMSEncoder?>) -> OSStatus

Creates a CMSEncoder reference.

func CMSEncoderCopyRecipients(CMSEncoder, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Obtains the array of recipients specified with the `CMSEncoderAddRecipients` function.

func CMSDecoderIsContentEncrypted(CMSDecoder, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Determines whether a CMS message was encrypted.

