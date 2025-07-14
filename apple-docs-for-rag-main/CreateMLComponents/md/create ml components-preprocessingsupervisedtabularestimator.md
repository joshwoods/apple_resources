

- Create ML Components
-  PreprocessingSupervisedTabularEstimator 

Structure

# PreprocessingSupervisedTabularEstimator

A supervised tabular estimator that composes a preprocessing transformer and a supervised tabular estimator.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
struct PreprocessingSupervisedTabularEstimator where Preprocessor : TabularTransformer, Estimator : SupervisedTabularEstimator
```

## Topics

### Creating an estimator

init(Preprocessor, Estimator)

Creates a composed supervised tabular estimator from a preprocessing transformer and a supervised tabular estimator.

### Getting the properties

var annotationColumnID: ColumnID&lt;Estimator.Annotation>

The annotation column identifier.

var estimator: Estimator

The estimator.

var preprocessor: Preprocessor

The preprocessing transformer.

### Encoding and decoding

func decode(from: inout any EstimatorDecoder) throws -> PreprocessingSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Decodes a previously fitted transformer.

func encode(PreprocessingSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

### Preprocesing and fitting

func preprocessed(from: DataFrame, eventHandler: EventHandler?) async throws -> DataFrame

Preprocesses a data frame of examples.

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a data frame

func fitted(toPreprocessed: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> PreprocessingSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Fits a transformer to a data frame of preprocessed examples while validating.

typealias Annotation

The annotation type.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

SupervisedTabularEstimator Implementations

## Relationships

### Conforms To

- Sendable
- SupervisedTabularEstimator

## See Also

### Tabular components

protocol TabularTransformer

A tabular transformer that transforms a data frame.

protocol TabularEstimator

A tabular estimator that creates a transformer by fitting to a data set in a data frame.

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

struct PreprocessingTabularEstimator

An estimator that composes a preprocessing transformer and an estimator.

struct PreprocessingUpdatableSupervisedTabularEstimator

An updatable supervised estimator that composes a preprocessing transformer and an updatable supervised estimator.

struct PreprocessingUpdatableTabularEstimator

An updatable estimator that composes a preprocessing transformer and an updatable estimator.

