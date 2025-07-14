

- Create ML Components
- TemporalTransformer
-  OutputSequence 

Associated Type

# OutputSequence

The output async sequence type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
associatedtype OutputSequence : TemporalSequence
```

**Required**

## See Also

### Applying and adapting

func applied&lt;S>(to: S, eventHandler: EventHandler?) async throws -> Self.OutputSequence

Performs the transformation on an input sequence.

**Required** Default implementations provided.

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

