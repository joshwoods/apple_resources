

- RealityKit
- NetworkCompatibilityToken
-  init(from:) 

Initializer

# init(from:)

Creates a new instance from a decoder.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS

``` source
required init(from decoder: any Decoder) throws
```

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

Throws an error if reading from `decoder` fails, or if the data is corrupted or otherwise invalid.

## See Also

### Serializing tokens

func encode(to: any Encoder) throws

Writes the token’s data into an encoder.

