

- AppKit
-  NSColorSpace 

Class

# NSColorSpace

An object that represents a custom color space.

macOS

``` source
class NSColorSpace
```

## Overview

You can make custom color spaces from ColorSync profiles or from ICC profiles. NSColorSpace also has factory methods that return objects representing the system color spaces.

You can use the init(colorSpace:components:count:) method of the NSColor class to create color objects using custom NSColorSpace objects. You can also send the usingColorSpace(_:) message to an NSColor object to convert it between two color spaces, either of which may be a custom color space.

## Topics

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

class var adobeRGB1998: NSColorSpace

A color space object that represents an Adobe RGB (1998) color space.

### Getting the Color Spaces Available On the System

class func availableColorSpaces(with: NSColorSpace.Model) -> [NSColorSpace]

Returns the list of color spaces available on the system that are displayed in the color panel, in the order they are displayed in the color panel.

### Initializing a Custom Color Space Object

init?(cgColorSpace: CGColorSpace)

Initializes and returns a color space object initialized from a Core Graphics color-space object.

init?(colorSyncProfile: UnsafeMutableRawPointer)

Initializes and returns a color space object from the specified ColorSync profile.

init?(iccProfileData: Data)

Initializes and returns a color space object from the specified ICC profile.

### Accessing Color Space Data and Attributes

var cgColorSpace: CGColorSpace?

The Core Graphics color-space object that represents a color space equivalent to the color space’s.

var colorSpaceModel: NSColorSpace.Model

The model on which the color space is based.

enum Model

Constants that describe the abstract model on which color space objects are based.

var colorSyncProfile: UnsafeMutableRawPointer?

The ColorSync profile from which the color space was created.

var iccProfileData: Data?

The ICC profile data from which the color space was created.

var localizedName: String?

The localized name of the color space.

var numberOfColorComponents: Int

The number of components, excluding alpha, the color space supports.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Colors

class NSColor

An object that stores color data and sometimes opacity (alpha value).

class NSColorList

An ordered list of color objects, identified by keys.

