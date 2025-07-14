

- Create ML Components
- Transformer
-  callAsFunction(\_:eventHandler:) 

Instance Method

# callAsFunction(\_:eventHandler:)

Performs the transformation on a sequence of inputs.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func callAsFunction(
    _ input: S,
    eventHandler: EventHandler? = nil
) async throws -> [Self.Output] where S : Sequence, Self.Input == S.Element
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

func callAsFunction(Self.Input, eventHandler: EventHandler?) async throws -> Self.Output

Performs the transformation on a single input.

func prediction&lt;S, Label>(from: S) async throws -> [ClassificationDistribution&lt;Label>]

Performs a prediction from a sequence of inputs.

func prediction&lt;Label>(from: Self.Input) async throws -> ClassificationDistribution&lt;Label>

Performs a prediction from a single input.

func prediction&lt;S, Annotation>(from: S, eventHandler: EventHandler?) async throws -> [AnnotatedPrediction&lt;Self.Output, Annotation>]

Performs a prediction on a sequence of annotated inputs.

