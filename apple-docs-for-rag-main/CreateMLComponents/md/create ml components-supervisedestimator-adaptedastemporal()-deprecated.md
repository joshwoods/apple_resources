

- Create ML Components
- SupervisedEstimator
-  adaptedAsTemporal() Deprecated

Instance Method

# adaptedAsTemporal()

Exposes this supervised estimator as a temporal supervised estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func adaptedAsTemporal() -> SupervisedEstimatorToTemporalAdaptor
```

Available when `Annotation` conforms to `Sendable`.

## See Also

### Adapting and fitting

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples.

**Required** Default implementation provided.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

**Required** Default implementation provided.

func fitted&lt;Input>(to: Input) async throws -> Self.Transformer

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation) async throws -> Self.Transformer

