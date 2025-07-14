

- Create ML Components
- UpdatableSupervisedEstimator
-  writeWithOptimizer(\_:to:overwrite:) 

Instance Method

# writeWithOptimizer(\_:to:overwrite:)

Writes the encoded transformer and optimizer to a file.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

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

## See Also

### Reading and writing

func readWithOptimizer(from: URL) throws -> Self.Transformer

Reads the encoded transformer and optimizer from a file.

