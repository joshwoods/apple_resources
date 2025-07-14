

- Create ML Components
- SupervisedTemporalEstimator
-  Annotation Deprecated

Associated Type

# Annotation

The annotation type.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
associatedtype Annotation : Equatable, Sendable
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

associatedtype Transformer : TemporalTransformer

The transformer type created by this estimator.

**Required**

Deprecated

