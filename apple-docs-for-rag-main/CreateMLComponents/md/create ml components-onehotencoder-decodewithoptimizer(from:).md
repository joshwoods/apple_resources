

- Create ML Components
- OneHotEncoder
-  decodeWithOptimizer(from:) 

Instance Method

# decodeWithOptimizer(from:)

Reads the encoded transformer with a decoder.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func decodeWithOptimizer(from decoder: inout any EstimatorDecoder) throws -> OneHotEncoder.Transformer
```

Available when `Category` conforms to `Comparable`, `Decodable`, `Encodable`, and `Hashable`.

## Parameters 

`decoder`  

A decoder.

## Return Value

The decoded transformer.

