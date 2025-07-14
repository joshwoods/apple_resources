

- Create ML Components
- TemporalTransformer
-  adaptedAsUpdatableEstimator() Deprecated

Instance Method

# adaptedAsUpdatableEstimator()

Exposes this temporal transformer as a trivial temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func adaptedAsUpdatableEstimator() -> TemporalTransformerToUpdatableEstimatorAdaptor
```

## See Also

### Applying and adapting

func applied&lt;S>(to: S, eventHandler: EventHandler?) async throws -> Self.OutputSequence

Performs the transformation on an input sequence.

**Required** Default implementations provided.

func adaptedAsEstimator() -> TemporalTransformerToEstimatorAdaptor&lt;Self>

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

