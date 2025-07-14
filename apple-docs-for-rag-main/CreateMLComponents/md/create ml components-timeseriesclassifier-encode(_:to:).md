

- Create ML Components
- TimeSeriesClassifier
-  encode(\_:to:) 

Instance Method

# encode(\_:to:)

Encodes a fitted encodable transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func encode(
    _ transformer: Self.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

Available when `Transformer` conforms to `Encodable`.

## Parameters 

`transformer`  

A transformer created by this estimator.

`encoder`  

An estimator encoder.

