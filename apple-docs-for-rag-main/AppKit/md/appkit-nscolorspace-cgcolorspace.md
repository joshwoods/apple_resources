

- AppKit
- NSColorSpace
-  cgColorSpace 

Instance Property

# cgColorSpace

The Core Graphics color-space object that represents a color space equivalent to the color space’s.

macOS 10.5+

``` source
var cgColorSpace: CGColorSpace? { get }
```

## Discussion

The value of this property is a reference to an Core Graphics color-space object (CGColorSpace) or `NULL` if the type of color space represented by the receiver cannot be represented by a `CGColorSpace` object.

## See Also

### Accessing Color Space Data and Attributes

var colorSpaceModel: NSColorSpace.Model

The model on which the color space is based.

enum Model

Constants that describe the abstract model on which color space objects are based.

var colorSyncProfile: UnsafeMutableRawPointer?

The ColorSync profile from which the color space was created.

var iccProfileData: Data?

The ICC profile data from which the color space was created.

var localizedName: String?

The localized name of the color space.

var numberOfColorComponents: Int

The number of components, excluding alpha, the color space supports.

