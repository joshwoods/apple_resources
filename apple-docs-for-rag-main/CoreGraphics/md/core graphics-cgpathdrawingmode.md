

- Core Graphics
-  CGPathDrawingMode 

Enumeration

# CGPathDrawingMode

Options for rendering a path.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGPathDrawingMode
```

## Overview

You can pass a path drawing mode constant to the function drawPath(using:) to specify how Core Graphics should paint a graphics context’s current path.

## Topics

### Constants

case fill

Render the area contained within the path using the non-zero winding number rule.

case eoFill

Render the area within the path using the even-odd rule.

case stroke

Render a line along the path.

case fillStroke

First fill and then stroke the path, using the nonzero winding number rule.

case eoFillStroke

First fill and then stroke the path, using the even-odd rule.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Drawing the Current Graphics Path

func drawPath(using: CGPathDrawingMode)

Draws the current path using the provided drawing mode.

func fillPath(using: CGPathFillRule)

Paints the area within the current path, as determined by the specified fill rule.

func strokePath()

Paints a line along the current path.

