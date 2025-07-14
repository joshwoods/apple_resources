

- Core Graphics
-  CGColorSpaceModel 

Enumeration

# CGColorSpaceModel

Models for color spaces.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGColorSpaceModel
```

## Topics

### Constants

case unknown

An unknown color space model.

case monochrome

A monochrome color space model.

case rgb

An RGB color space model.

case cmyk

A CMYK color space model.

case lab

A Lab color space model.

case deviceN

A DeviceN color space model.

case indexed

An indexed color space model.

case pattern

A pattern color space model.

case XYZ

An XYZ color space model.

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

### Examining a Color Space

var baseColorSpace: CGColorSpace?

Returns the base color space of a pattern or indexed color space.

var numberOfComponents: Int

Returns the number of color components in a color space.

var model: CGColorSpaceModel

Returns the color space model of the provided color space.

var colorTable: [UInt8]?

The entries in the color table of an indexed color space.

func copyICCData() -> CFData?

Returns a copy of the ICC profile data of the provided color space.

func copyPropertyList() -> CFPropertyList?

Returns a copy of the color space’s properties.

var iccData: CFData?

Returns a copy of the ICC profile of the provided color space.

Deprecated

var name: CFString?

Returns the name used to create the specified color space.

var supportsOutput: Bool

Returns a Boolean indicating whether the color space can be used as a destination color space.

var isWideGamutRGB: Bool

Returns whether the RGB color space covers a significant portion of the NTSC color gamut.

