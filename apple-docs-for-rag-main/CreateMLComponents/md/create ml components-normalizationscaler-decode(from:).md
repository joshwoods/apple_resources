

- Create ML Components
- NormalizationScaler
-  decode(from:) 

Instance Method

# decode(from:)

Decodes a previously fitted decodable transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> Self.Transformer
```

Available when `Transformer` conforms to `Decodable`.

## Parameters 

`decoder`  

An estimator decoder.

## Return Value

The decoded transformer.

