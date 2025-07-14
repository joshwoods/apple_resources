

- Create ML Components
-  EstimatorEncoder 

Protocol

# EstimatorEncoder

A type that can encode values into a model representation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
protocol EstimatorEncoder
```

## Topics

### Encoding values

func encode&lt;T>(T) throws

Encodes a value.

**Required**

func encodeOptimizer&lt;T>(T) throws

Encodes an estimator optimizer.

**Required**

## See Also

### Serializers

protocol EstimatorDecoder

A type that can decode values from a model representation.

