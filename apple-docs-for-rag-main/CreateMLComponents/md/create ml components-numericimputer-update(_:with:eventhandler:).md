

- Create ML Components
- NumericImputer
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates an impute transformer with a new sequence of examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout ImputeTransformer,
    with input: some Sequence>,
    eventHandler: EventHandler? = nil
) throws
```

Available when `Element` conforms to `BinaryFloatingPoint`, `Decodable`, and `Encodable`.

## Parameters 

`transformer`  

A transformer to update.

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## Discussion

Note

You can’t update an impute transformer when using the `median` strategy.

