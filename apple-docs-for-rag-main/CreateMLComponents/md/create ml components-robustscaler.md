

- Create ML Components
-  RobustScaler 

Structure

# RobustScaler

An estimator that scales the input using statistics that are robust to outliers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct RobustScaler where Element : BinaryFloatingPoint, Element : Decodable, Element : Encodable
```

## Topics

### Creating an estimator

init(quantileRange: ClosedRange&lt;Element>)

Creates a robust scaler.

### Getting the properties

var quantileRange: ClosedRange&lt;Element>

The quantile range used to compute the scale.

### Fitting

func fitted&lt;S>(to: S, eventHandler: EventHandler?) throws -> RobustScaler&lt;Element>.Transformer

Fits a robust scaler to a sequence of elements.

### Default Implementations

Estimator Implementations

## Relationships

### Conforms To

- Estimator
- Sendable

## See Also

### Scalers

struct StandardScaler

An estimator that standardizes the input by removing the mean and scaling to unit variance.

struct MaxAbsScaler

An estimator that scales the input values so that the maximum absolute value is 1.0.

struct MinMaxScaler

An estimator that scales the input values so that they all lie in a closed range.

struct NormalizationScaler

An estimator that normalizes the input values using a normalization strategy.

