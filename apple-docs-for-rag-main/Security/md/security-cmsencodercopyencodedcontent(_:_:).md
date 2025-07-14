

- Security
-  CMSEncoderCopyEncodedContent(\_:\_:) 

Function

# CMSEncoderCopyEncodedContent(\_:\_:)

Finishes encoding the message and obtains the encoded result.

macOS 10.5+

``` source
func CMSEncoderCopyEncodedContent(
    _ cmsEncoder: CMSEncoder,
    _ encodedContentOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the `CMSEncoderCreate` function.

`encodedContentOut`  

On return, points to the encoded message. You must use the `CFRelease` function to free this reference when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This is the last function in the sequence of encoding functions you call when creating a signed or encrypted message. In many cases, you can call the `CMSEncode` function alone instead of using the sequence of encoding functions.

