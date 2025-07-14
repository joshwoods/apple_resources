

- Create ML Components
-  StandardScaler 

Structure

# StandardScaler

An estimator that standardizes the input by removing the mean and scaling to unit variance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct StandardScaler where Element : BinaryFloatingPoint, Element : Decodable, Element : Encodable
```

## Topics

### Creating an estimator

init()

Creates a standard scaling estimator.

### Fitting

func fitted&lt;S>(to: S, eventHandler: EventHandler?) throws -> StandardScaler&lt;Element>.Transformer

Fits a transformer to a particular input sequence by computing the mean and standard deviation.

### Default Implementations

Estimator Implementations

UpdatableEstimator Implementations

## Relationships

### Conforms To

- Copyable
- Estimator
- Sendable
- UpdatableEstimator

  Conforms when `Element` conforms to `BinaryFloatingPoint`, `Decodable`, and `Encodable`.

## See Also

### Scalers

struct MaxAbsScaler

An estimator that scales the input values so that the maximum absolute value is 1.0.

struct MinMaxScaler

An estimator that scales the input values so that they all lie in a closed range.

struct NormalizationScaler

An estimator that normalizes the input values using a normalization strategy.

struct RobustScaler

An estimator that scales the input using statistics that are robust to outliers.

