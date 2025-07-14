

- Core Graphics
-  CGLineCap 

Enumeration

# CGLineCap

Styles for rendering the endpoint of a stroked line.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGLineCap
```

## Overview

A line cap specifies the method used by strokePath() to draw the endpoint of the line. To change the line cap style in a graphics context, you use the function setLineCap(_:).

## Topics

### Constants

case butt

A line with a squared-off end. Core Graphics draws the line to extend only to the exact endpoint of the path. This is the default.

case round

A line with a rounded end. Core Graphics draws the line to extend beyond the endpoint of the path. The line ends with a semicircular arc with a radius of 1/2 the line’s width, centered on the endpoint.

case square

A line with a squared-off end. Core Graphics extends the line beyond the endpoint of the path for a distance equal to half the line width.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

