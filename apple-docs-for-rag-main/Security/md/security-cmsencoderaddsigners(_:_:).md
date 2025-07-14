

- Security
-  CMSEncoderAddSigners(\_:\_:) 

Function

# CMSEncoderAddSigners(\_:\_:)

Specifies signers of the message.

macOS 10.5+

``` source
func CMSEncoderAddSigners(
    _ cmsEncoder: CMSEncoder,
    _ signerOrArray: CFTypeRef
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the `CMSEncoderCreate` function.

`signerOrArray`  

The identity object for the identity of one signer, specified as type `SecIdentityRef`, or a `CFArray` of identity objects of type`SecIdentityRef`.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Call this function only if the message is to be signed. You can call this function more than once for the same message.

If you do call this function, you must call it before the first call to the CMSEncoderUpdateContent(_:_:_:) function.

## See Also

### Related Documentation

func CMSEncoderUpdateContent(CMSEncoder, UnsafeRawPointer, Int) -> OSStatus

Feeds content bytes into the encoder.

func CMSEncoderCopySigners(CMSEncoder, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Obtains the array of signers specified with the `CMSEncoderAddSigners` function.

func CMSEncoderCreate(UnsafeMutablePointer&lt;CMSEncoder?>) -> OSStatus

Creates a CMSEncoder reference.

func CMSDecoderCopySignerStatus(CMSDecoder, Int, CFTypeRef, Bool, UnsafeMutablePointer&lt;CMSSignerStatus>?, UnsafeMutablePointer&lt;SecTrust?>?, UnsafeMutablePointer&lt;OSStatus>?) -> OSStatus

Obtains the status of a CMS message’s signature.

