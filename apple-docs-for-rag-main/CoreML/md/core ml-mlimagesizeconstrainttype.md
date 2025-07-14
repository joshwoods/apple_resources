

- Core ML
-  MLImageSizeConstraintType 

Enumeration

# MLImageSizeConstraintType

The modes that determine how the model defines a feature’s image size constraint.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum MLImageSizeConstraintType
```

## Topics

### Enumeration Cases

case range

The image feature accepts image sizes defined by a range of widths and a range of heights.

case enumerated

The image feature accepts image sizes listed in an array.

case unspecified

The image size constraint is not configured and should be ignored.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining Relevant Constraints

var type: MLImageSizeConstraintType

Indicator of which properties to inspect for this image size constraint.

