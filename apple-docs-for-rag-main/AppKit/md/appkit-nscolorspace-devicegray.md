

- AppKit
- NSColorSpace
-  deviceGray 

Type Property

# deviceGray

A color space object that represents a calibrated or device-dependent gray color space.

macOS

``` source
class var deviceGray: NSColorSpace { get }
```

## Return Value

The `NSColorSpace` object. The color space also includes an alpha component. Typical devices that use this color space are grayscale printers and displays. This object corresponds to the Cocoa color space name `NSDeviceWhiteColorSpace`.

## See Also

### Getting a Named Color Space

class var deviceRGB: NSColorSpace

A color space object that represents a calibrated or device-dependent RGB color space.

class var genericRGB: NSColorSpace

A color space object that represents a device-independent RGB color space.

class var deviceCMYK: NSColorSpace

A color space object that represents a calibrated or device-dependent CMYK color space.

class var genericCMYK: NSColorSpace

A color space object that represents a device-independent CMYK color space.

class var genericGray: NSColorSpace

A color space object that represents a device-independent gray color space.

class var sRGB: NSColorSpace

A color space object that represents an sRGB color space.

class var extendedSRGB: NSColorSpace

A color space object that represents an extended sRGB color space.

class var displayP3: NSColorSpace

A color space object that represents a P3 Display color space.

class var genericGamma22Gray: NSColorSpace

A color space object that represents a gray color space with a gamma value of 2.2.

class var extendedGenericGamma22Gray: NSColorSpace

A color space object that represents an extended gray color space with a gamma value of 2.2.

class var adobeRGB1998: NSColorSpace

A color space object that represents an Adobe RGB (1998) color space.

