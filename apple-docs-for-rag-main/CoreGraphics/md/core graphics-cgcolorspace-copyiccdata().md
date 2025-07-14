

- Core Graphics
- CGColorSpace
-  copyICCData() 

Instance Method

# copyICCData()

Returns a copy of the ICC profile data of the provided color space.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func copyICCData() -> CFData?
```

## Return Value

The ICC profile data or `NULL` if the color space does not have an ICC data profile.

## See Also

### Examining a Color Space

var baseColorSpace: CGColorSpace?

Returns the base color space of a pattern or indexed color space.

var numberOfComponents: Int

Returns the number of color components in a color space.

var model: CGColorSpaceModel

Returns the color space model of the provided color space.

enum CGColorSpaceModel

Models for color spaces.

var colorTable: [UInt8]?

The entries in the color table of an indexed color space.

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

