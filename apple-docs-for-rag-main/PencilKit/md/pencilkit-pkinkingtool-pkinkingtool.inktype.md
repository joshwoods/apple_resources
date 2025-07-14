

- PencilKit
- PKInkingTool
-  PKInkingTool.InkType 

Enumeration

# PKInkingTool.InkType

The type that defines the shape of stroked lines.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
enum InkType
```

## Topics

### Choosing ink types

case marker

An inking tool that creates the appearance of a felt-tip marker.

case pen

An inking tool that creates the appearance of a pen-based drawing.

case pencil

An inking tool that creates the appearance of a narrow line from a pencil.

case monoline

An inking tool that creates the appearance of a monoline pen.

case fountainPen

An inking tool that creates the appearance of a calligraphy pen.

case watercolor

An inking tool that creates the appearance of a watercolor brush.

case crayon

An inking tool that creates the appearance of a crayon.

### Getting the width information

var defaultWidth: CGFloat

The default line width for the specified tool type.

var validWidthRange: ClosedRange&lt;CGFloat>

The range of widths allowed for an ink of this type.

### Supporting backward compatibility

var requiredContentVersion: PKContentVersion

The version of PencilKit necessary to use the ink type.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Getting the tool type

var inkType: PKInkingTool.InkType

The tool type that determines the shape of the rendered content.

