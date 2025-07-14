

- Security
-  CMSEncoderCopyRecipients(\_:\_:) 

Function

# CMSEncoderCopyRecipients(\_:\_:)

Obtains the array of recipients specified with the `CMSEncoderAddRecipients` function.

macOS 10.5+

``` source
func CMSEncoderCopyRecipients(
    _ cmsEncoder: CMSEncoder,
    _ recipientsOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the CMSEncoderCreate(_:) function.

`recipientsOut`  

On return, points to an array of certificate objects of type SecCertificate of the recipients of the message. If the CMSEncoderAddRecipients(_:_:) function has not been called for this message, this function returns a `NULL` array. You must use the CFRelease function to free this reference when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## See Also

### Related Documentation

func CMSEncoderCreate(UnsafeMutablePointer&lt;CMSEncoder?>) -> OSStatus

Creates a CMSEncoder reference.

func CMSEncoderAddRecipients(CMSEncoder, CFTypeRef) -> OSStatus

Specifies a message is to be encrypted and specifies the recipients of the message.

