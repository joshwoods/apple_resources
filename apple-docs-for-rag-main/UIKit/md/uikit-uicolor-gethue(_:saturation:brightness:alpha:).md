

- UIKit
- UIColor
-  getHue(\_:saturation:brightness:alpha:) 

Instance Method

# getHue(\_:saturation:brightness:alpha:)

Returns the components that form the color in the HSB color space.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func getHue(
    _ hue: UnsafeMutablePointer?,
    saturation: UnsafeMutablePointer?,
    brightness: UnsafeMutablePointer?,
    alpha: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`hue`  

On return, the hue component of the color object. On applications linked for iOS 10 or later, an extended range color space specifies the hue component and can have any value. Values between `0.0` and `1.0` are inside the sRGB color gamut. On earlier versions of iOS, the specified value is always between `0.0` and `1.0`.

`saturation`  

On return, the saturation component of the color object. On applications linked for iOS 10 or later, an extended range color space specifies and can have any value. Values between `0.0` and `1.0` are inside the sRGB color gamut. On earlier versions of iOS, the specified value is always between `0.0` and `1.0`.

`brightness`  

On return, the brightness component of the color object. On applications linked for iOS 10 or later, an extended range color space specifies the brightness component and can have any value. Values between `0.0` and `1.0` are inside the sRGB color gamut. On earlier versions of iOS, the specified value is always between `0.0` and `1.0`.

`alpha`  

On return, the opacity component of the color object, specified as a value between `0.0` and `1.0`.

## Return Value

true if the color could be converted, false otherwise.

## Discussion

If the color is in a compatible color space, it converts into the HSB color space, and its components return to your application. If the color isn’t in a compatible color space, the parameters don’t change.

## See Also

### Getting the color information

Determining color values with color spaces

Change the system’s interpretation of a color value for display by selecting a color space.

var cgColor: CGColor

The Quartz color that corresponds to the color object.

var ciColor: CIColor

The Core Image color that corresponds to the color object.

func getRed(UnsafeMutablePointer&lt;CGFloat>?, green: UnsafeMutablePointer&lt;CGFloat>?, blue: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the components that form the color in the RGB color space.

func getWhite(UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the grayscale components of the color.

var accessibilityName: String

A localized description of the color for accessibility attributes.

