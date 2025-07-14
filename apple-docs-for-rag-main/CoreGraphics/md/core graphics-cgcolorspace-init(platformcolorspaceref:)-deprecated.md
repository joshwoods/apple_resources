

- Core Graphics
- CGColorSpace
-  init(platformColorSpaceRef:) Deprecated

Initializer

# init(platformColorSpaceRef:)

Creates a platform-specific color space.

iOS 9.0–15.0DeprecatediPadOS 9.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.0–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–8.0Deprecated

``` source
init?(platformColorSpaceRef ref: UnsafeRawPointer)
```

Deprecated

No longer supported

## Parameters 

`ref`  

A generic pointer to a platform-specific color space. In macOS, pass a `ColorSyncProfileRef`, which is a ColorSync profile. Quartz uses this pointer (and the underlying information) only during the function call.

## Return Value

A new color space, or `NULL` if unsuccessful. In Objective-C, you’re responsible for releasing this object by calling CGColorSpaceRelease.

## Discussion

Colors in a device-dependent color space are not transformed or otherwise modified when displayed on an output device — that is, there is no attempt to maintain the visual appearance of a color. As a consequence, colors in a device color space often appear different when displayed on different output devices. For this reason, device color spaces are not recommended when color preservation is important.

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

init?(labWhitePoint: UnsafePointer&lt;CGFloat>, blackPoint: UnsafePointer&lt;CGFloat>?, range: UnsafePointer&lt;CGFloat>?)

Creates a device-independent color space that is relative to human color perception, according to the CIE L\*a\*b\* standard.

init?(patternBaseSpace: CGColorSpace?)

Creates a pattern color space.

init?(name: CFString)

Creates a specified type of Quartz color space.

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

