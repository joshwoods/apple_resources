

- Security
-  CMSEncoderAddSignedAttributes(\_:\_:) 

Function

# CMSEncoderAddSignedAttributes(\_:\_:)

Specifies attributes for a signed message.

macOS 10.5+

``` source
func CMSEncoderAddSignedAttributes(
    _ cmsEncoder: CMSEncoder,
    _ signedAttributes: CMSSignedAttributes
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the `CMSEncoderCreate` function.

`signedAttributes`  

Attribute flags as defined in CMSSignedAttributes.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Attributes are optional for signed messages. They are not used for other types of CMS messages. The use of attributes is described in section 2.5 of the S/MIME 3.1 specification.

If you do call this function, you must call it before the first call to the CMSEncoderUpdateContent(_:_:_:) function.

## See Also

### Related Documentation

func CMSEncoderUpdateContent(CMSEncoder, UnsafeRawPointer, Int) -> OSStatus

Feeds content bytes into the encoder.

func CMSEncoderCreate(UnsafeMutablePointer&lt;CMSEncoder?>) -> OSStatus

Creates a CMSEncoder reference.

