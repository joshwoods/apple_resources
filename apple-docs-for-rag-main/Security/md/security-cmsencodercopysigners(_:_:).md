

- Security
-  CMSEncoderCopySigners(\_:\_:) 

Function

# CMSEncoderCopySigners(\_:\_:)

Obtains the array of signers specified with the `CMSEncoderAddSigners` function.

macOS 10.5+

``` source
func CMSEncoderCopySigners(
    _ cmsEncoder: CMSEncoder,
    _ signersOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the CMSEncoderCreate(_:) function.

`signersOut`  

On return, points to an array of identity objects of type SecIdentity of the signers of the message. If the CMSEncoderAddSigners(_:_:) function has not been called for this message, this function returns a `NULL` array. You must use the CFRelease function to free this reference when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## See Also

### Related Documentation

func CMSEncoderCreate(UnsafeMutablePointer&lt;CMSEncoder?>) -> OSStatus

Creates a CMSEncoder reference.

func CMSEncoderAddSigners(CMSEncoder, CFTypeRef) -> OSStatus

Specifies signers of the message.

