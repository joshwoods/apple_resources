

- Create ML Components
- FullyConnectedNetworkMultiLabelClassifierModel
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs a classification on a shaped array.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func applied(
    to input: MLShapedArray,
    eventHandler: EventHandler? = nil
) throws -> ClassificationDistribution
```

## Parameters 

`input`  

The classifier input.

`eventHandler`  

An event handler.

## Return Value

A classification distribution.

