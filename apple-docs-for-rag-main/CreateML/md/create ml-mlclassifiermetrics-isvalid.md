

- Create ML
- MLClassifierMetrics
-  isValid 

Instance Property

# isValid

A Boolean value indicating whether the classifier model was able to calculate metrics.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var isValid: Bool { get }
```

## Discussion

Your metrics may be invalid if you attempt to perform evaluation on data that doesn’t match the structure of your training examples.

## See Also

### Handling errors

var error: (any Error)?

The underlying error present when the metrics are invalid.

