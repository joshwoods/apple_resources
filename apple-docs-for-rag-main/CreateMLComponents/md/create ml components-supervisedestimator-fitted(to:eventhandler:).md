

- Create ML Components
- SupervisedEstimator
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Fits a transformer to a sequence of examples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: Input,
    eventHandler: EventHandler?
) async throws -> Self.Transformer where Input : Sequence, Input.Element == AnnotatedFeature
```

**Required** Default implementation provided.

## Parameters 

`input`  

A sequence of examples used for fitting the transformer.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## Default Implementations

### SupervisedEstimator Implementations

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to an async sequence of examples.

## See Also

### Adapting and fitting

func adaptedAsTemporal() -> SupervisedEstimatorToTemporalAdaptor&lt;Self>

Exposes this supervised estimator as a temporal supervised estimator.

Deprecated

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

**Required** Default implementation provided.

func fitted&lt;Input>(to: Input) async throws -> Self.Transformer

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation) async throws -> Self.Transformer

