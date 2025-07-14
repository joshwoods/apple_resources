

- Core Graphics
-  CGLineJoin 

Enumeration

# CGLineJoin

Junction types for stroked lines.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGLineJoin
```

## Overview

A line join specifies how strokePath() draws the junction between connected line segments. To set the line join style in a graphics context, you use the function setLineJoin(_:).

## Topics

### Constants

case miter

case round

A join with a rounded end. Core Graphics draws the line to extend beyond the endpoint of the path. The line ends with a semicircular arc with a radius of 1/2 the line’s width, centered on the endpoint.

case bevel

A join with a squared-off end. Core Graphics draws the line to extend beyond the endpoint of the path, for a distance of 1/2 the line’s width.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

