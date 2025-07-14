

- Core Graphics
- CGColorSpace
-  init(labWhitePoint:blackPoint:range:) 

Initializer

# init(labWhitePoint:blackPoint:range:)

Creates a device-independent color space that is relative to human color perception, according to the CIE L\*a\*b\* standard.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    labWhitePoint whitePoint: UnsafePointer,
    blackPoint: UnsafePointer?,
    range: UnsafePointer?
)
```

## Parameters 

`whitePoint`  

An array of 3 numbers that specify the tristimulus value, in the CIE 1931 XYZ-space, of the diffuse white point.

`blackPoint`  

An array of 3 numbers that specify the tristimulus value, in CIE 1931 XYZ-space, of the diffuse black point.

`range`  

An array of 4 numbers that specify the range of valid values for the a\* and b\* components of the color space. The a\* component represents values running from green to red, and the b\* component represents values running from blue to yellow.

## Return Value

A new L\*a\*b\* color space, or `NULL` if unsuccessful. In Objective-C, you’re responsible for releasing this object by calling CGColorSpaceRelease.

## Discussion

The CIE L\*a\*b\* space is a nonlinear transformation of the Munsell color notation system (a system which specifies colors by hue, value, and saturation—or “chroma”—values), designed to match perceived color difference with quantitative distance in color space. The L\* component represents the lightness value, the a\* component represents values running from green to red, and the b\* component represents values running from blue to yellow. This roughly corresponds to the way the human brain is thought to decode colors. Colors in a device-independent color space should appear the same when displayed on different devices, to the extent that the capabilities of the device allow.

## See Also

### Creating Color Spaces

init?(calibratedGrayWhitePoint: UnsafePointer&lt;CGFloat>, blackPoint: UnsafePointer&lt;CGFloat>?, gamma: CGFloat)

Creates a calibrated grayscale color space.

init?(calibratedRGBWhitePoint: UnsafePointer&lt;CGFloat>, blackPoint: UnsafePointer&lt;CGFloat>?, gamma: UnsafePointer&lt;CGFloat>?, matrix: UnsafePointer&lt;CGFloat>?)

Creates a calibrated RGB color space.

init?(iccBasedNComponents: Int, range: UnsafePointer&lt;CGFloat>?, profile: CGDataProvider, alternate: CGColorSpace?)

Creates a device-independent color space that is defined according to the ICC color profile specification.

init?(indexedBaseSpace: CGColorSpace, last: Int, colorTable: UnsafePointer&lt;UInt8>)

Creates an indexed color space, consisting of colors specified by a color lookup table.

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

