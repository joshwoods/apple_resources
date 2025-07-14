

- Create ML Components
- SupervisedTemporalEstimator
-  write(\_:to:overwrite:) Deprecated

Instance Method

# write(\_:to:overwrite:)

Writes the encoded transformer to a file.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func write(
    _ transformer: Self.Transformer,
    to url: URL,
    overwrite: Bool = true
) throws
```

## Parameters 

`transformer`  

A transformer created by this estimator.

`url`  

A file URL.

`overwrite`  

A Boolean value indicating whether to overwrite existing files.

## See Also

### Reading and writing

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

Deprecated

associatedtype Annotation : Equatable, Sendable

The annotation type.

**Required**

Deprecated

associatedtype Transformer : TemporalTransformer

The transformer type created by this estimator.

**Required**

Deprecated

