

- Create ML Components
- SupervisedTabularEstimator
-  annotationColumnID 

Instance Property

# annotationColumnID

The annotation column identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var annotationColumnID: ColumnID { get set }
```

**Required**

## See Also

### Reading and writing

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

associatedtype Annotation

The annotation type.

**Required**

associatedtype Transformer : TabularTransformer

The transformer type created by this estimator.

**Required**

