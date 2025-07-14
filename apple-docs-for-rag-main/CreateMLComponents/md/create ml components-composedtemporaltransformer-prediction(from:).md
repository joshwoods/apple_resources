

- Create ML Components
- ComposedTemporalTransformer
-  prediction(from:) 

Instance Method

# prediction(from:)

Performs a prediction on a single input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func prediction(from input: S) async throws -> Self.OutputSequence where S : TemporalSequence, Label : Hashable, Self.Input == S.Feature, Self.Output == ClassificationDistribution
```

## Parameters 

`input`  

The input feature.

## Return Value

A classification array.

