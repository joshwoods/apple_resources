

- Security
-  CMSDecoderUpdateMessage(\_:\_:\_:) 

Function

# CMSDecoderUpdateMessage(\_:\_:\_:)

Feeds raw bytes of the message to be decoded into the decoder.

macOS 10.5+

``` source
func CMSDecoderUpdateMessage(
    _ cmsDecoder: CMSDecoder,
    _ msgBytes: UnsafeRawPointer,
    _ msgBytesLen: Int
) -> OSStatus
```

## Parameters 

`cmsDecoder`  

The CMSDecoder reference returned by the `CMSDecoderCreate` function.

`msgBytes`  

A pointer to the data to be decoded.

`msgBytesLen`  

The length of the data, in bytes.

## Return Value

A result code. See Security Framework Result Codes. Returns errSecUnknownFormat upon detection of an improperly formatted CMS message.

## Discussion

This function can be called multiple times. Call the `CMSDecoderFinalizeMessage` function when you have no more data to decode.

## See Also

### Related Documentation

func CMSDecoderCreate(UnsafeMutablePointer&lt;CMSDecoder?>) -> OSStatus

Creates a CMSDecoder reference.

