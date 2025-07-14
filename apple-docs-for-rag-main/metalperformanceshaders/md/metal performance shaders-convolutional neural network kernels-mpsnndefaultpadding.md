

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSNNDefaultPadding 

Class

# MPSNNDefaultPadding

A class that provides predefined padding policies for common tasks.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSNNDefaultPadding : NSObject
```

## Topics

### Initializers

init(method: MPSNNPaddingMethod)

struct MPSNNPaddingMethod

Options that define a graph's padding.

### Instance Methods

func label() -> String

### Type Methods

class func forTensorflowAveragePooling() -> Self

class func forTensorflowAveragePoolingValidOnly() -> Self

## Relationships

### Inherits From

- NSObject

### Conforms To

- MPSNNPadding

