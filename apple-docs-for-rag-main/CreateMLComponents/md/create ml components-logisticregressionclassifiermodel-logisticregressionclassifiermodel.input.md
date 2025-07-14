

- Create ML Components
- LogisticRegressionClassifierModel
-  LogisticRegressionClassifierModel.Input 

Type Alias

# LogisticRegressionClassifierModel.Input

The input type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Input = MLShapedArray
```

## See Also

### Performing the classification

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) async throws -> ClassificationDistribution&lt;Label>

Performs a classification on a single input.

