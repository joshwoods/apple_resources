

- Core ML
-  MLImageSizeConstraint 

Class

# MLImageSizeConstraint

A list or range of sizes that augment an image constraint’s default size.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class MLImageSizeConstraint
```

## Overview

You use an `MLImageSizeConstraint` to express what image sizes of an image feature a model will accept as input or produce as output.

Use type to determine which properties describe what image sizes the model’s image feature expects as input or produces as output.

If `type` is:

- MLImageSizeConstraintType.range, the image feature accepts any image that has a width in pixelsWideRange and a height in pixelsHighRange.

- MLImageSizeConstraintType.enumerated, the image feature accepts any image size listed in enumeratedImageSizes.

- MLImageSizeConstraintType.unspecified, the `MLImageSizeConstraint` instance is not configured and should be ignored. Instead, use the image feature’s default image size constraint, defined by pixelsWide and pixelsHigh.

## Topics

### Determining Relevant Constraints

var type: MLImageSizeConstraintType

Indicator of which properties to inspect for this image size constraint.

enum MLImageSizeConstraintType

The modes that determine how the model defines a feature’s image size constraint.

### Accessing the Image Size Ranges

var pixelsWideRange: NSRange

The range of widths a model’s image feature accepts as input or produces as output.

var pixelsHighRange: NSRange

The range of heights a model’s image feature accepts as input or produces as output.

### Accessing the Enumerated Image Sizes

var enumeratedImageSizes: [MLImageSize]

An array of image sizes a model’s image feature accepts as input or produces as output.

class MLImageSize

The width and height of an image feature size.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Inspecting Acceptable Sizes

var sizeConstraint: MLImageSizeConstraint

Additional sizes this image feature supports.

