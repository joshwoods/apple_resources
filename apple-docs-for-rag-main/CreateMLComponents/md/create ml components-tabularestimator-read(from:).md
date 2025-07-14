

- Create ML Components
- TabularEstimator
-  read(from:) 

Instance Method

# read(from:)

Reads the encoded transformer from a file.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

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

associatedtype Transformer : TabularTransformer

The transformer type created by this estimator.

**Required**

