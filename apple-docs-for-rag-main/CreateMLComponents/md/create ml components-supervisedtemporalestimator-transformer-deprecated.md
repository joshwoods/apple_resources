

- Create ML Components
- SupervisedTemporalEstimator
-  Transformer Deprecated

Associated Type

# Transformer

The transformer type created by this estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
associatedtype Transformer : TemporalTransformer
```

**Required**

## See Also

### Reading and writing

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

Deprecated

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

Deprecated

associatedtype Annotation : Equatable, Sendable

The annotation type.

**Required**

Deprecated

