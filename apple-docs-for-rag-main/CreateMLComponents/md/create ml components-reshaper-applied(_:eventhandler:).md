

- Create ML Components
- Reshaper
-  applied(\_:eventHandler:) 

Instance Method

# applied(\_:eventHandler:)

Reshapes a sequence of inputs.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    _ input: S,
    eventHandler: EventHandler? = nil
) throws -> [MLShapedArray] where S : Sequence, S.Element == MLShapedArray
```

## Parameters 

`input`  

A sequence of input shaped arrays.

`eventHandler`  

An event handler.

## Return Value

An array of shaped arrays.

## See Also

### Performing the transformation

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) throws -> MLShapedArray&lt;Scalar>

Reshapes the input.

