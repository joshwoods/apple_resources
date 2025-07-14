

- Create ML Components
- EstimatorEncoder
-  encodeOptimizer(\_:) 

Instance Method

# encodeOptimizer(\_:)

Encodes an estimator optimizer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
mutating func encodeOptimizer(_ value: T) throws where T : Encodable
```

**Required**

## Discussion

Optimizers are used when fitting an estimator and usually contain state information such as momentum. This method encodes the optimizer state separately from model parameters.

## See Also

### Encoding values

func encode&lt;T>(T) throws

Encodes a value.

**Required**

