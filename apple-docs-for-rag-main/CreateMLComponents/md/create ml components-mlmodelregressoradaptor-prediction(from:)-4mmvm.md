

- Create ML Components
- MLModelRegressorAdaptor
-  prediction(from:) 

Instance Method

# prediction(from:)

Performs a prediction from a sequence of inputs.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func prediction(from input: S) async throws -> [Self.Output] where S : Sequence, Self.Input == S.Element
```

## Parameters 

`input`  

The input features.

## Return Value

An array of regressions.

