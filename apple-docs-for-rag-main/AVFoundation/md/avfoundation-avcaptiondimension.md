

- AVFoundation
-  AVCaptionDimension 

Structure

# AVCaptionDimension

A structure that defines a caption dimension.

iOSiPadOSMac CatalystmacOS

``` source
struct AVCaptionDimension
```

## Topics

### Inspecting the Dimensions

var value: CGFloat

The value of the coordinate or length.

var units: AVCaptionUnitsType

The units of the coordinate, such as cells or points.

enum AVCaptionUnitsType

A structure that defines a units for caption formats.

### Initializers

init()

Creates a caption dimension.

init(value: CGFloat, units: AVCaptionUnitsType)

Creates a caption dimension with a value and unit type.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

