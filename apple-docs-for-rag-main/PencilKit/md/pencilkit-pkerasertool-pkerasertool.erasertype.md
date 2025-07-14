

- PencilKit
- PKEraserTool
-  PKEraserTool.EraserType 

Enumeration

# PKEraserTool.EraserType

Constants that indicate the behavior of the eraser.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
enum EraserType
```

## Topics

### Eraser types

case vector

An eraser that removes an entire drawn line.

case bitmap

An eraser that removes only those portions of the drawing it touches.

case fixedWidthBitmap

### Getting the width information

var defaultWidth: CGFloat

The default width for an eraser type.

var validWidthRange: ClosedRange&lt;CGFloat>

The valid width range for an eraser type.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Getting the eraser type

var eraserType: PKEraserTool.EraserType

The behavior adopted by the eraser when deleting content.

