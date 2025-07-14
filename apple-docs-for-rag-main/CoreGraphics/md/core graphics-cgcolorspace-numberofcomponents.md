

- Core Graphics
- CGColorSpace
-  numberOfComponents 

Instance Property

# numberOfComponents

Returns the number of color components in a color space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var numberOfComponents: Int { get }
```

## Discussion

A color space defines an n-dimensional space whose dimensions (or components) represent intensity values. Use this function to obtain the number of components in a given color space: for example, in an RGB color space this function returns 3 (for the three intensity values red, green, and blue).

## See Also

### Examining a Color Space

var baseColorSpace: CGColorSpace?

Returns the base color space of a pattern or indexed color space.

var model: CGColorSpaceModel

Returns the color space model of the provided color space.

enum CGColorSpaceModel

Models for color spaces.

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

