

- Security
-  CMSEncoderUpdateContent(\_:\_:\_:) 

Function

# CMSEncoderUpdateContent(\_:\_:\_:)

Feeds content bytes into the encoder.

macOS 10.5+

``` source
func CMSEncoderUpdateContent(
    _ cmsEncoder: CMSEncoder,
    _ content: UnsafeRawPointer,
    _ contentLen: Int
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the `CMSEncoderCreate` function.

`content`  

The content that you want to add to the message. The content must conform to the type set with the CMSEncoderSetEncapsulatedContentType function (or type `id-data` if that function has not been called).

`contentLen`  

The length of the content being added, in bytes.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

You use this function to add the content that is to be signed or encrypted. If the message is only a container for certificates added with the CMSEncoderAddSupportingCerts(_:_:) function and has no other content, do not call this function. This function can be called multiple times.

After you are finished adding content, call the `CMSEncoderCopyEncodedContent` function to complete the message creation process.

None of the setter functions (CMSEncoderSetHasDetachedContent(_:_:), CMSEncoderSetEncapsulatedContentType, or CMSEncoderSetCertificateChainMode(_:_:)) can be called after this function has been called.

