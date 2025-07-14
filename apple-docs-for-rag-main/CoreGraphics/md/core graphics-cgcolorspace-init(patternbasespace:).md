

- Core Graphics
- CGColorSpace
-  init(patternBaseSpace:) 

Initializer

# init(patternBaseSpace:)

Creates a pattern color space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(patternBaseSpace baseSpace: CGColorSpace?)
```

## Parameters 

`baseSpace`  

For masking patterns, the underlying color space that specifies the colors to be painted through the mask. For color patterns, you should pass `NULL`.

## Return Value

A new pattern color space, or `NULL` if unsuccessful. In Objective-C, you’re responsible for releasing this object by calling CGColorSpaceRelease.

## Discussion

For information on creating and using patterns, see Quartz 2D Programming Guide and CGPattern. Quartz retains the color space you pass in. Upon return, you may safely release it by calling CGColorSpaceRelease.

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

