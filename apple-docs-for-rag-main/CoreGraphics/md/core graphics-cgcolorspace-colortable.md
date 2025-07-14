

- Core Graphics
- CGColorSpace
-  colorTable 

Instance Property

# colorTable

The entries in the color table of an indexed color space.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var colorTable: [UInt8]? { get }
```

## Discussion

If the color space is an indexed color space, this array contains color component values for the colors in the color space, in the same format you use when creating an indexed color space with the init(indexedBaseSpace:last:colorTable:) initializer.

If the color space is not an indexed color space, this property’s value is `nil`. To determine whether a color space is an indexed color space, read the model property.

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

