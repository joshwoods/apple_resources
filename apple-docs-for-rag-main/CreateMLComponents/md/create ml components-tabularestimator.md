

- Create ML Components
-  TabularEstimator 

Protocol

# TabularEstimator

A tabular estimator that creates a transformer by fitting to a data set in a data frame.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
protocol TabularEstimator
```

## Topics

### Reading and writing

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

associatedtype Transformer : TabularTransformer

The transformer type created by this estimator.

**Required**

### Appending

func appending&lt;Other>(Other) -> some TabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>> 

Compose this tabular estimator with another tabular estimator.

func appending&lt;Other>(Other) -> some TabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other>> 

Compose this tabular estimator with a tabular transformer.

func appending&lt;Other>(Other) -> some SupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this tabular estimator with a supervised tabular estimator.

### Adapting and fitting

func adaptedAsSupervised&lt;Annotation>(annotationColumnID: ColumnID&lt;Annotation>) -> TabularEstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this tabular estimator as a supervised tabular estimator.

func fitted(to: DataFrame, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a data frame

**Required**

### Encoding and decoding

func encode(Self.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

**Required** Default implementation provided.

func decode(from: inout any EstimatorDecoder) throws -> Self.Transformer

Decodes a previously fitted transformer.

**Required** Default implementation provided.

### Instance Methods

func fitted(to: DataFrame) async throws -> Self.Transformer

func fitted(to: DataFrame) async throws -> Self.Transformer

## Relationships

### Inherited By

- UpdatableTabularEstimator

### Conforming Types

- ColumnSelector
- PreprocessingTabularEstimator
- PreprocessingUpdatableTabularEstimator
- TabularTransformerToEstimatorAdaptor
- TabularTransformerToUpdatableEstimatorAdaptor

## See Also

### Tabular components

protocol TabularTransformer

A tabular transformer that transforms a data frame.

protocol SupervisedTabularEstimator

A tabular estimator that creates a transformer by fitting to a data set in a data frame.

struct ColumnSelector

An operation that applies an estimator to a selection of columns.

struct ColumnSelectorTransformer

A transformer that applies a base transformer to specific columns in a data frame.

enum ColumnSelection

A selection of columns from a data frame.

struct ColumnConcatenator

A transformer that concatenates every numerical column in a dataframe into to a shaped array for each row.

struct PreprocessingSupervisedTabularEstimator

A supervised tabular estimator that composes a preprocessing transformer and a supervised tabular estimator.

struct PreprocessingTabularEstimator

An estimator that composes a preprocessing transformer and an estimator.

struct PreprocessingUpdatableSupervisedTabularEstimator

An updatable supervised estimator that composes a preprocessing transformer and an updatable supervised estimator.

struct PreprocessingUpdatableTabularEstimator

An updatable estimator that composes a preprocessing transformer and an updatable estimator.

