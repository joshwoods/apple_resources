

- Create ML Components
- LogisticRegressionClassifier
-  LogisticRegressionClassifier.Configuration 

Structure

# LogisticRegressionClassifier.Configuration

A logistic regression classifier configuration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct Configuration
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

## Topics

### Creating a configuration

init()

Creates a default logistic regression classifier configuration.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Getting the properties

var convergenceThreshold: Double

The convergence threshold.

var earlyStopIterationCount: Int

The number of iterations to use when evaluating whether to stop early.

var l1Penalty: Double

Weight of the L1 regularization term.

var l2Penalty: Double

Weight of the L2 regularization term.

var maximumIterations: Int

The maximum number of allowed passes through the data.

var optimizationStrategy: OptimizationStrategy

The optimization strategy.

var scaleFeatures: Bool

A Boolean value indicating whether to scale the input features.

var stepSize: Double

The starting step size to use for the solver.

### Operators

static func == (LogisticRegressionClassifier&lt;Scalar, Label>.Configuration, LogisticRegressionClassifier&lt;Scalar, Label>.Configuration) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a classifier

init(labels: Set&lt;Label>, configuration: LogisticRegressionClassifier&lt;Scalar, Label>.Configuration)

Creates a logistic regression classifier.

