

- Create ML Components
- Transformer
-  prediction(from:) 

Instance Method

# prediction(from:)

Performs a prediction from a single input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func prediction(from input: Self.Input) async throws -> ClassificationDistribution where Label : Hashable, Self.Output == ClassificationDistribution
```

## Parameters 

`input`  

The input feature.

## Return Value

A classification array.

## See Also

### Transforming and predicting

func callAsFunction(Self.Input, eventHandler: EventHandler?) async throws -> Self.Output

Performs the transformation on a single input.

func callAsFunction&lt;S>(S, eventHandler: EventHandler?) async throws -> [Self.Output]

Performs the transformation on a sequence of inputs.

func prediction&lt;S, Label>(from: S) async throws -> [ClassificationDistribution&lt;Label>]

Performs a prediction from a sequence of inputs.

func prediction&lt;S, Annotation>(from: S, eventHandler: EventHandler?) async throws -> [AnnotatedPrediction&lt;Self.Output, Annotation>]

Performs a prediction on a sequence of annotated inputs.

