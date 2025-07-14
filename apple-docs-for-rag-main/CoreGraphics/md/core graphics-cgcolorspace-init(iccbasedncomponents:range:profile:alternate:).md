

- Core Graphics
- CGColorSpace
-  init(iccBasedNComponents:range:profile:alternate:) 

Initializer

# init(iccBasedNComponents:range:profile:alternate:)

Creates a device-independent color space that is defined according to the ICC color profile specification.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    iccBasedNComponents nComponents: Int,
    range: UnsafePointer?,
    profile: CGDataProvider,
    alternate: CGColorSpace?
)
```

## Parameters 

`nComponents`  

The number of color components in the color space defined by the ICC profile data. This must match the number of components actually in the ICC profile and must equal 1, 3, or 4.

`range`  

An array of numbers that specify the minimum and maximum valid values of the corresponding color components. The size of the array is two times the number of components. If `c[k]` is the `k`the color component, the valid range is range`[2*k] ≤ c[k] ≤` range`[2*k+1]`.

`profile`  

A data provider that supplies the ICC profile.

`alternate`  

An alternate color space to use in case the ICC profile is not supported. The alternate color space must have `nComponents` color components. You must supply an alternate color space. If this parameter is `NULL`, then the function returns `NULL`.

## Return Value

A new ICC-based color space object, or `NULL` if unsuccessful. In Objective-C, you’re responsible for releasing this object by calling CGColorSpaceRelease.

## Discussion

This function creates an ICC-based color space from an ICC color profile, as defined by the International Color Consortium. ICC profiles define the reproducible color gamut (the range of colors supported by a device) and other characteristics of a particular output device, providing a way to accurately transform the color space of one device to the color space of another. The ICC profile is usually provided by the manufacturer of the device. Additionally, some color monitors and printers contain electronically embedded ICC profile information, as do some bitmap formats such as TIFF. Colors in a device-independent color space should appear the same when displayed on different devices, to the extent that the capabilities of the device allow.

You may want to use this function for a color space that requires a detailed gamma, such as the piecewise transfer function used in sRGB or ITU-R BT.709, because this function can accurately represent these gamma curves.

## See Also

### Creating Color Spaces

init?(calibratedGrayWhitePoint: UnsafePointer&lt;CGFloat>, blackPoint: UnsafePointer&lt;CGFloat>?, gamma: CGFloat)

Creates a calibrated grayscale color space.

init?(calibratedRGBWhitePoint: UnsafePointer&lt;CGFloat>, blackPoint: UnsafePointer&lt;CGFloat>?, gamma: UnsafePointer&lt;CGFloat>?, matrix: UnsafePointer&lt;CGFloat>?)

Creates a calibrated RGB color space.

init?(indexedBaseSpace: CGColorSpace, last: Int, colorTable: UnsafePointer&lt;UInt8>)

Creates an indexed color space, consisting of colors specified by a color lookup table.

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

