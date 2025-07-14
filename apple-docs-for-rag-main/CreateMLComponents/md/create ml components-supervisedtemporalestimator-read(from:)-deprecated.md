

- Create ML Components
- SupervisedTemporalEstimator
-  read(from:) Deprecated

Instance Method

# read(from:)

Reads the encoded transformer from a file.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func read(from url: URL) throws -> Self.Transformer
```

## Parameters 

`url`  

A file URL.

## Return Value

The decoded transformer.

## See Also

### Reading and writing

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

Deprecated

associatedtype Annotation : Equatable, Sendable

The annotation type.

**Required**

Deprecated

associatedtype Transformer : TemporalTransformer

The transformer type created by this estimator.

**Required**

Deprecated

