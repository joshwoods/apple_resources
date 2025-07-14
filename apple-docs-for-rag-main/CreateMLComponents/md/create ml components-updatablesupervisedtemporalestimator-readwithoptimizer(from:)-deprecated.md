

- Create ML Components
- UpdatableSupervisedTemporalEstimator
-  readWithOptimizer(from:) Deprecated

Instance Method

# readWithOptimizer(from:)

Reads the encoded transformer and optimizer from a file.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func readWithOptimizer(from url: URL) throws -> Self.Transformer
```

## Parameters 

`url`  

A file URL.

## Return Value

The decoded transformer.

## See Also

### Reading and writing

func writeWithOptimizer(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer and optimizer to a file.

Deprecated

