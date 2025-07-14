

- UIKit
- Drawing
- UIColor
-  Determining color values with color spaces 

Article

# Determining color values with color spaces

Change the system’s interpretation of a color value for display by selecting a color space.

## Overview

A UIColor object typically stores its color value as a Core Graphics color (CGColor) in a Core Graphics color space (CGColorSpace). When creating a custom color, the underlying color space and the range of values for each color component vary based on the iOS version.

### Create colors with color spaces

For apps running on iOS 9 and earlier, colors use one of two color spaces:

- Device-dependent Gray

- Device-dependent RGB

These device color spaces correspond closely to the display characteristics of the sRGB color space. Component values within these color spaces are in the range `0.0` to `1.0`. When you create a color, the color object clamps values to ensure they fit within this range.

### Use extended color spaces

For apps running on iOS 10 or later, colors use the following extended color spaces:

- extendedGray

- extendedSRGB

In the extended color spaces, UIColor doesn’t clamp values to fit inside the color gamut. Component values may be less than `0.0` or greater than `1.0`. On an sRGB display, such colors are outside the gamut and won’t render accurately. However, the extended color spaces are useful when you want a pixel format and representation that extended color spaces can convert into other color spaces. For example, you can still convert color in the display P3 color space to an extended sRGB format, even if that color isn’t within the sRGB color gamut. When you convert such a color, some of its values fall outside the `0.0` to `1.0` range. However, the color still renders correctly on a device with a P3 display gamut.

When employing custom colors, use extended color spaces to store your color values. When representing a color as closely as possible, convert the color from the extended color space into the target color space.

## See Also

### Getting the color information

var cgColor: CGColor

The Quartz color that corresponds to the color object.

var ciColor: CIColor

The Core Image color that corresponds to the color object.

func getHue(UnsafeMutablePointer&lt;CGFloat>?, saturation: UnsafeMutablePointer&lt;CGFloat>?, brightness: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the components that form the color in the HSB color space.

func getRed(UnsafeMutablePointer&lt;CGFloat>?, green: UnsafeMutablePointer&lt;CGFloat>?, blue: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the components that form the color in the RGB color space.

func getWhite(UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the grayscale components of the color.

var accessibilityName: String

A localized description of the color for accessibility attributes.

