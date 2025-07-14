

- ML Compute
-  MLCPlatform Deprecated

Class

# MLCPlatform

A utility class for setting global properties in the framework.

iOS 15.0–17.4DeprecatediPadOS 15.0–17.4DeprecatedMac Catalyst 15.0–17.4DeprecatedmacOS 12.0–14.3DeprecatedtvOS 15.0–17.4Deprecated

``` source
class MLCPlatform
```

## Topics

### Getting the RNG Seed

class func getRNGseed() -> NSNumber?

Returns the global random number generator seed value.

### Setting the RNG Seed

class func setRNGSeedTo(NSNumber)

Sets the global random number generator seed value.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Components

class MLCTensor

The data object you use throughout the framework.

Deprecated

Layers

Create and inspect layers that encapsulate operations and configuration details to receive, process, and output tensors.

Training and Validation

Create, train, and validate a graph to produce acceptable prediction results.

