

- Core ML
-  MLMetricKey 

Class

# MLMetricKey

A key for the metrics dictionary in an update context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
class MLMetricKey
```

## Topics

### Getting the Keys

class var lossValue: MLMetricKey

The key you use to access the current loss (a `float` value).

class var epochIndex: MLMetricKey

The key you use to access the epoch index (an `Int64` value).

class var miniBatchIndex: MLMetricKey

The key you use to access the mini-batch index (an `Int64` value) within an epoch.

### Supporting Types

class MLKey

An abstract base class for machine learning key types.

## Relationships

### Inherits From

- MLKey

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Evaluating the Update

var metrics: [MLMetricKey : Any]

The training metrics of the model for the update task, contained in a dictionary.

