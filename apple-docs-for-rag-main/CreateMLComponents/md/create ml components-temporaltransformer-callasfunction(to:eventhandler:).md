

- Create ML Components
- TemporalTransformer
-  callAsFunction(to:eventHandler:) 

Instance Method

# callAsFunction(to:eventHandler:)

Performs the transformation on a sequence of inputs.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func callAsFunction(
    to input: S,
    eventHandler: EventHandler? = nil
) async throws -> [Self.OutputSequence] where S : Sequence, Self.Input == S.Element.Feature, S.Element : TemporalSequence
```

## Parameters 

`input`  

The transformer inputs.

`eventHandler`  

An event handler.

## Return Value

The outputs produced by applying the transformer to the inputs.

## See Also

### Transforming and predicting

func callAsFunction&lt;S>(S, eventHandler: EventHandler?) async throws -> Self.OutputSequence

Performs the transformation on an input sequence.

func prediction&lt;S, Label>(from: S) async throws -> Self.OutputSequence

Performs a prediction on a single input.

