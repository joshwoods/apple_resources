

- Create ML
- MLCheckpoint
-  init(from:) 

Initializer

# init(from:)

Creates a new checkpoint by decoding from the decoder.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
init(from decoder: any Decoder) throws
```

## Parameters 

`decoder`  

The decoder to read data from.

## See Also

### Encoding and decoding a checkpoint

func encode(to: any Encoder) throws

Encodes the checkpoint into the encoder.

