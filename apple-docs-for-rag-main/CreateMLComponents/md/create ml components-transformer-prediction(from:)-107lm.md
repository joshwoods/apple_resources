

- Create ML Components
- Transformer
-  prediction(from:) 

Instance Method

# prediction(from:)

Performs a prediction from a sequence of inputs.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func prediction(from input: S) async throws -> [ClassificationDistribution] where S : Sequence, Label : Hashable, Self.Input == S.Element, Self.Output == ClassificationDistribution
```

## Parameters 

`input`  

The input features.

## Return Value

An array of classification distributions.

## See Also

### Transforming and predicting

func callAsFunction(Self.Input, eventHandler: EventHandler?) async throws -> Self.Output

Performs the transformation on a single input.

func callAsFunction&lt;S>(S, eventHandler: EventHandler?) async throws -> [Self.Output]

Performs the transformation on a sequence of inputs.

func prediction&lt;Label>(from: Self.Input) async throws -> ClassificationDistribution&lt;Label>

Performs a prediction from a single input.

func prediction&lt;S, Annotation>(from: S, eventHandler: EventHandler?) async throws -> [AnnotatedPrediction&lt;Self.Output, Annotation>]

Performs a prediction on a sequence of annotated inputs.

