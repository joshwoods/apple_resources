

- AVFoundation
-  AVCaptionUnitsType 

Enumeration

# AVCaptionUnitsType

A structure that defines a units for caption formats.

iOSiPadOSMac CatalystmacOS

``` source
enum AVCaptionUnitsType
```

## Overview

Some geometry values may use sizing and positioning with different units. In some cases, an object might allow multiple kinds of dimensions varying by units.

## Topics

### Unit Types

case cells

A cell-based unit type.

case percent

A percentage-based unit type.

case unspecified

An unspecified unit type.

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

### Inspecting the Dimensions

var value: CGFloat

The value of the coordinate or length.

var units: AVCaptionUnitsType

The units of the coordinate, such as cells or points.

