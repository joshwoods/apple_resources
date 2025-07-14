

- Create ML Components
- Transformer
-  prediction(from:eventHandler:) 

Instance Method

# prediction(from:eventHandler:)

Performs a prediction on a sequence of annotated inputs.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func prediction(
    from input: S,
    eventHandler: EventHandler? = nil
) async throws -> [AnnotatedPrediction] where S : Sequence, S.Element == AnnotatedFeature
```

## Parameters 

`input`  

A sequence of annotated inputs.

`eventHandler`  

An event handler.

## Return Value

Annotated predictions produced by applying the transformer to the inputs.

## See Also

### Transforming and predicting

func callAsFunction(Self.Input, eventHandler: EventHandler?) async throws -> Self.Output

Performs the transformation on a single input.

func callAsFunction&lt;S>(S, eventHandler: EventHandler?) async throws -> [Self.Output]

Performs the transformation on a sequence of inputs.

func prediction&lt;S, Label>(from: S) async throws -> [ClassificationDistribution&lt;Label>]

Performs a prediction from a sequence of inputs.

func prediction&lt;Label>(from: Self.Input) async throws -> ClassificationDistribution&lt;Label>

Performs a prediction from a single input.

