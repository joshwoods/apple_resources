

- Create ML Components
-  EstimatorDecoder 

Protocol

# EstimatorDecoder

A type that can decode values from a model representation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
protocol EstimatorDecoder
```

## Topics

### Decoding values

func decode&lt;T>(T.Type) throws -> T

Decodes a value.

**Required**

func decodeOptimizer&lt;T>(T.Type) throws -> T

Decodes an optimizer value.

**Required**

## See Also

### Serializers

protocol EstimatorEncoder

A type that can encode values into a model representation.

