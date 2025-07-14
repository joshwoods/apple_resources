

- Create ML Components
- UpdatableEstimatorToSupervisedAdaptor
-  SupervisedEstimator Implementations 

API Collection

# SupervisedEstimator Implementations

## Topics

### Instance Methods

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Self.Annotation> 

Composes this supervised estimator with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised estimator with another supervised estimator.

func appending&lt;Other>(Other) -> some SupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised estimator with an estimator.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other>, Self.Annotation> 

Composes this supervised estimator with a temporal transformer.

Deprecated

func appending&lt;Other>(Other) -> some SupervisedEstimator&lt;ComposedTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this supervised estimator with a transformer.

func appending&lt;Other>(Other) -> some SupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self.Transformer>, Other.Transformer>, Self.Annotation> 

Composes this supervised estimator with a temporal estimator.

Deprecated

func fitted&lt;Input>(to: Input) async throws -> Self.Transformer

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to an async sequence of examples.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation) async throws -> Self.Transformer

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to an async sequence of examples while validating with a validation sequence.

func read(from: URL) throws -> Self.Transformer

Reads the encoded transformer from a file.

func write(Self.Transformer, to: URL, overwrite: Bool) throws

Writes the encoded transformer to a file.

