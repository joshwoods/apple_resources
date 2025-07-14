

- Core Graphics
- CGColorSpace
-  init(indexedBaseSpace:last:colorTable:) 

Initializer

# init(indexedBaseSpace:last:colorTable:)

Creates an indexed color space, consisting of colors specified by a color lookup table.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    indexedBaseSpace baseSpace: CGColorSpace,
    last lastIndex: Int,
    colorTable: UnsafePointer
)
```

## Parameters 

`baseSpace`  

The color space on which the color table is based.

`lastIndex`  

The maximum valid index value for the color table. The value must be less than or equal to 255.

`colorTable`  

An array of `m*(lastIndex+1)` bytes, where `m` is the number of color components in the base color space. Each byte is an unsigned integer in the range `0` to `255` that is scaled to the range of the corresponding color component in the base color space.

## Return Value

A new indexed color space object, or `NULL` if unsuccessful. In Objective-C, you’re responsible for releasing this object by calling CGColorSpaceRelease.

## Discussion

An indexed color space contains a color table with up to 255 entries, and a base color space to which the color table entries are mapped. Each entry in the color table specifies one color in the base color space. A value in an indexed color space is treated as an index into the color table of the color space. The data in the table is in meshed format. (For example, for an RGB color space the values are R, G, B, R, G, B, and so on.)

## See Also

### Creating Color Spaces

init?(calibratedGrayWhitePoint: UnsafePointer&lt;CGFloat>, blackPoint: UnsafePointer&lt;CGFloat>?, gamma: CGFloat)

Creates a calibrated grayscale color space.

init?(calibratedRGBWhitePoint: UnsafePointer&lt;CGFloat>, blackPoint: UnsafePointer&lt;CGFloat>?, gamma: UnsafePointer&lt;CGFloat>?, matrix: UnsafePointer&lt;CGFloat>?)

Creates a calibrated RGB color space.

init?(iccBasedNComponents: Int, range: UnsafePointer&lt;CGFloat>?, profile: CGDataProvider, alternate: CGColorSpace?)

Creates a device-independent color space that is defined according to the ICC color profile specification.

init?(labWhitePoint: UnsafePointer&lt;CGFloat>, blackPoint: UnsafePointer&lt;CGFloat>?, range: UnsafePointer&lt;CGFloat>?)

Creates a device-independent color space that is relative to human color perception, according to the CIE L\*a\*b\* standard.

init?(patternBaseSpace: CGColorSpace?)

Creates a pattern color space.

init?(name: CFString)

Creates a specified type of Quartz color space.

init?(platformColorSpaceRef: UnsafeRawPointer)

Creates a platform-specific color space.

Deprecated

init?(iccData: CFTypeRef)

Creates an ICC-based color space using the ICC profile contained in the specified data.

init?(propertyListPlist: CFPropertyList)

Creates a color space from a property list.

func CGColorSpaceCreateDeviceRGB() -> CGColorSpace

Creates a device-dependent RGB color space.

func CGColorSpaceCreateDeviceCMYK() -> CGColorSpace

Creates a device-dependent CMYK color space.

func CGColorSpaceCreateDeviceGray() -> CGColorSpace

Creates a device-dependent grayscale color space.

init?(iccProfileData: CFData)

Creates an ICC-based color space using the ICC profile contained in the specified data.

Deprecated

