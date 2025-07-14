

- Metal Performance Shaders
-  MPSMatrixRandomDistributionDescriptor 

Class

# MPSMatrixRandomDistributionDescriptor

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MPSMatrixRandomDistributionDescriptor : NSObject
```

## Topics

### Instance Properties

var distributionType: MPSMatrixRandomDistribution

var maximum: Float

var mean: Float

var minimum: Float

var standardDeviation: Float

### Type Methods

class func `default`() -> MPSMatrixRandomDistributionDescriptor

class func normalDistributionDescriptor(withMean: Float, standardDeviation: Float) -> MPSMatrixRandomDistributionDescriptor

class func normalDistributionDescriptor(withMean: Float, standardDeviation: Float, minimum: Float, maximum: Float) -> MPSMatrixRandomDistributionDescriptor

class func uniformDistributionDescriptor(withMinimum: Float, maximum: Float) -> MPSMatrixRandomDistributionDescriptor

## Relationships

### Inherits From

- NSObject

### Conforms To

- NSCopying

