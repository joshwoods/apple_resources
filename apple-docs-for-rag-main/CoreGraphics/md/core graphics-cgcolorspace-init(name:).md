

- Core Graphics
- CGColorSpace
-  init(name:) 

Initializer

# init(name:)

Creates a specified type of Quartz color space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(name: CFString)
```

## Parameters 

`name`  

A color space name. See Accessing System-Defined Color Spaces for a list of the valid Quartz-defined names.

## Return Value

A new generic color space, or `NULL` if unsuccessful. In Objective-C, you’re responsible for releasing this object by calling CGColorSpaceRelease.

## Discussion

You can use this function to create a generic color space. For more information, see Accessing System-Defined Color Spaces.

## See Also

### Related Documentation

var name: CFString?

Returns the name used to create the specified color space.

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

