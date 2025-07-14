

- Vision
-  VNElementType 

Enumeration

# VNElementType

An enumeration of the type of element in feature print data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
enum VNElementType
```

## Topics

### Element Types

case unknown

The element type isn’t known.

case float

The elements are floating-point numbers.

case double

The elements are double-precision floating-point numbers.

### Creating an Element Type

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining Types of Feature Prints

var elementType: VNElementType

The type of each element in the data.

func VNElementTypeSize(VNElementType) -> Int

Returns the size of a feature print element.

