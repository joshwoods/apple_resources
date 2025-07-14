

- Create ML Components
-  NormalizationScaler 

Structure

# NormalizationScaler

An estimator that normalizes the input values using a normalization strategy.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct NormalizationScaler where Element : BinaryFloatingPoint, Element : Decodable, Element : Encodable
```

## Topics

### Creating a scaler

init(norm: NormalizationScaler&lt;Element>.NormalizationStrategy)

Creates a normalization scaler.

enum NormalizationStrategy

A normalization strategy.

### Getting the normalization

var norm: NormalizationScaler&lt;Element>.NormalizationStrategy

The normalization strategy.

### Fitting

func fitted&lt;S>(to: S, eventHandler: EventHandler?) throws -> NormalizationScaler&lt;Element>.Transformer

Fits a normalization scaler to a sequence of elements.

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

struct RobustScaler

An estimator that scales the input using statistics that are robust to outliers.

