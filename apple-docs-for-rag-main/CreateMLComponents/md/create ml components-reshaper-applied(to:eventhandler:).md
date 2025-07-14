

- Create ML Components
- Reshaper
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Reshapes the input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: MLShapedArray,
    eventHandler: EventHandler? = nil
) throws -> MLShapedArray
```

## Parameters 

`input`  

A shaped array.

`eventHandler`  

An event handler.

## Return Value

A shaped array with the target shape.

## See Also

### Performing the transformation

func applied&lt;S>(S, eventHandler: EventHandler?) throws -> [MLShapedArray&lt;Scalar>]

Reshapes a sequence of inputs.

