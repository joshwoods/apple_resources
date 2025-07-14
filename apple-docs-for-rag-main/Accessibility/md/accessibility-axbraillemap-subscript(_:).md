

- Accessibility
- AXBrailleMap
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the height of an individual pin on the braille display.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+macOS 12.2+tvOS 15.2+visionOS 1.0+watchOS 8.2+

``` source
subscript(point: CGPoint) -> Float { get set }
```

## Overview

Use this subscript to set or get the height of an individual pin. This subscript provides the same capabilities as using setHeight(_:at:) and height(at:).

## See Also

### Accessing dots

func setHeight(Float, at: CGPoint)

Sets the height of an individual pin on the braille display.

func height(at: CGPoint) -> Float

Retrieves the height of an individual pin on the braille display.

