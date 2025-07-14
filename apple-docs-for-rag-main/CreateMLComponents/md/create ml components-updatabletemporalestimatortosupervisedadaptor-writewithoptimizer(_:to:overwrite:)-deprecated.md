

- Create ML Components
- UpdatableTemporalEstimatorToSupervisedAdaptor
-  writeWithOptimizer(\_:to:overwrite:) Deprecated

Instance Method

# writeWithOptimizer(\_:to:overwrite:)

Writes the encoded transformer and optimizer to a file.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func writeWithOptimizer(
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

