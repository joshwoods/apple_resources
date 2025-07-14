

- Create ML Components
- LogisticRegressionClassifierModel
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs a classification on a single input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: MLShapedArray,
    eventHandler: EventHandler? = nil
) async throws -> ClassificationDistribution
```

## Parameters 

`input`  

The classifier input.

`eventHandler`  

An event handler.

## Return Value

A classification distribution.

## See Also

### Performing the classification

typealias Input

The input type.

