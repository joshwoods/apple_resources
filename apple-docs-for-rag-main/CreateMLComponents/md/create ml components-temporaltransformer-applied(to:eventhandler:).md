

- Create ML Components
- TemporalTransformer
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs the transformation on an input sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: S,
    eventHandler: EventHandler?
) async throws -> Self.OutputSequence where S : TemporalSequence, Self.Input == S.Feature
```

**Required** Default implementations provided.

## Parameters 

`input`  

The input temporal sequence.

`eventHandler`  

An event handler.

## Return Value

An async sequence produced by applying the transformation to the input.

## Default Implementations

### TemporalTransformer Implementations

func applied&lt;S, TS, Annotation>(to: S, eventHandler: EventHandler?) async throws -> [AnnotatedFeature&lt;Self.OutputSequence, Annotation>]

Performs the transformation on a sequence of annotated input sequences.

func applied&lt;S>(to: S, eventHandler: EventHandler?) async throws -> [Self.OutputSequence]

Performs the transformation on a sequence of input sequences.

## See Also

### Applying and adapting

func adaptedAsEstimator() -> TemporalTransformerToEstimatorAdaptor&lt;Self>

Exposes this temporal transformer as a trivial temporal estimator.

Deprecated

func adaptedAsUpdatableEstimator() -> TemporalTransformerToUpdatableEstimatorAdaptor&lt;Self>

Exposes this temporal transformer as a trivial temporal estimator.

Deprecated

associatedtype Input

The input type.

**Required**

associatedtype Output

The output type.

**Required**

associatedtype OutputSequence : TemporalSequence

The output async sequence type.

**Required**

