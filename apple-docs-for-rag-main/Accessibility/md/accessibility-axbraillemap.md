

- Accessibility
-  AXBrailleMap 

Class

# AXBrailleMap

A representation of a two-dimensional braille display.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+macOS 12.1+tvOS 15.2+visionOS 1.0+watchOS 8.2+

``` source
class AXBrailleMap
```

## Overview

A braille map object represents a two-dimensional braille display that’s connected to the current Apple device. By specifying the dot patterns in the braille map, you can change the content the user experiences. To render the data from the braille map to the display, implement AXBrailleMapRenderer.

## Topics

### Creating a braille map

init?(coder: NSCoder)

### Getting display dimensions

var dimensions: CGSize

The number of pins in each dimension of the braille display.

### Accessing dots

func setHeight(Float, at: CGPoint)

Sets the height of an individual pin on the braille display.

func height(at: CGPoint) -> Float

Retrieves the height of an individual pin on the braille display.

subscript(CGPoint) -> Float

Accesses the height of an individual pin on the braille display.

### Displaying images

func present(CGImage)

Converts the data from the image you specify into the braille map.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Braille maps

protocol AXBrailleMapRenderer

The interface for providing data for a braille map.

