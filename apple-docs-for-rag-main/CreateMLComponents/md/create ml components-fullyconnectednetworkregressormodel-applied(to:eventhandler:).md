

- Create ML Components
- FullyConnectedNetworkRegressorModel
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs regression on a shaped array.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: MLShapedArray,
    eventHandler: EventHandler? = nil
) async throws -> FullyConnectedNetworkRegressorModel.Target
```

## Parameters 

`input`  

The regressor input.

`eventHandler`  

An event handler.

## Return Value

A regression.

## See Also

### Performing a regression

typealias Target

