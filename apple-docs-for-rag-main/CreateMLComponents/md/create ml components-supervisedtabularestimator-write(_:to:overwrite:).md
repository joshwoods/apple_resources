

- Create ML Components
- SupervisedTabularEstimator
-  write(\_:to:overwrite:) 

Instance Method

# write(\_:to:overwrite:)

Writes the encoded transformer to a file.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

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

associatedtype Annotation

The annotation type.

**Required**

var annotationColumnID: ColumnID&lt;Self.Annotation>

The annotation column identifier.

**Required**

associatedtype Transformer : TabularTransformer

The transformer type created by this estimator.

**Required**

