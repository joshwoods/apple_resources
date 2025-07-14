

- Security
-  CMSDecoderCreate(\_:) 

Function

# CMSDecoderCreate(\_:)

Creates a CMSDecoder reference.

macOS 10.5+

``` source
func CMSDecoderCreate(_ cmsDecoderOut: UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`cmsDecoderOut`  

On return, points to a CMSDecoder reference. You must use the `CFRelease` function to free this reference when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This is the first function in a sequence of decoder functions that you call to get information from a CMS message. The other functions in the sequence require you to pass in the CMSDecoder reference returned by this function. The next function in the sequence is `CMSDecoderUpdateMessage`.

## See Also

### Related Documentation

func CMSDecoderUpdateMessage(CMSDecoder, UnsafeRawPointer, Int) -> OSStatus

Feeds raw bytes of the message to be decoded into the decoder.

