

- SecureElementCredential
- CredentialSessionWindowSceneEvent
-  init(from:) 

Initializer

# init(from:)

Creates a new instance by decoding from the given decoder.

SecureElementCredentialUIKitiOS 17.4+iPadOS 17.4+

``` source
init(from decoder: any Decoder) throws
```

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

This initializer throws an error if reading from the decoder fails, or if the data read is corrupted or otherwise invalid.

## See Also

### Encoding and decoding

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

