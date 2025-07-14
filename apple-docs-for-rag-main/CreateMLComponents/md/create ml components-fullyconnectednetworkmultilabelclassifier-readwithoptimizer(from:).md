

- Create ML Components
- FullyConnectedNetworkMultiLabelClassifier
-  readWithOptimizer(from:) 

Instance Method

# readWithOptimizer(from:)

Reads the encoded transformer and optimizer from a file.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func readWithOptimizer(from url: URL) throws -> Self.Transformer
```

## Parameters 

`url`  

A file URL.

## Return Value

The decoded transformer.

