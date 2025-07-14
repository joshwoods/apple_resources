

- AppKit
- NSColorSpace
-  adobeRGB1998 

Type Property

# adobeRGB1998

A color space object that represents an Adobe RGB (1998) color space.

macOS 10.5+

``` source
class var adobeRGB1998: NSColorSpace { get }
```

## Return Value

The `NSColorSpace` object. This color-additive color space has red, green, blue, and alpha components.

## Discussion

The Adobe RGB (1998) color space was designed to encompass most of the colors achievable on CMYK color printers, but by using RGB primary colors on a device such as the computer display. For more information on this color space, go to http://www.adobe.com/digitalimag/adobergb.html.

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

class var deviceGray: NSColorSpace

A color space object that represents a calibrated or device-dependent gray color space.

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

