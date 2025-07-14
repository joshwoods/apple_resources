

- AppKit
- NSColorSpace
-  NSColorSpace.Model 

Enumeration

# NSColorSpace.Model

Constants that describe the abstract model on which color space objects are based.

macOS

``` source
enum Model
```

## Topics

### Color Spaces

case unknown

An unknown color-space model.

case gray

The grayscale color-space model.

case rgb

The RGB (red-green-blue) color-space model.

case cmyk

The CMYK (cyan-magenta-yellow-black) color-space model.

case lab

The L\*a\*b\* device-independent color-space model, which represents colors relative to a reference white point.

case deviceN

The DeviceN color-space model from Adobe Systems, Inc.

case indexed

An indexed color space, which identifies discrete colors in a color list by index number.

case patterned

A pattern color space, which is a repeated image that creates a tiled pattern.

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

### Accessing Color Space Data and Attributes

var cgColorSpace: CGColorSpace?

The Core Graphics color-space object that represents a color space equivalent to the color space’s.

var colorSpaceModel: NSColorSpace.Model

The model on which the color space is based.

var colorSyncProfile: UnsafeMutableRawPointer?

The ColorSync profile from which the color space was created.

var iccProfileData: Data?

The ICC profile data from which the color space was created.

var localizedName: String?

The localized name of the color space.

var numberOfColorComponents: Int

The number of components, excluding alpha, the color space supports.

