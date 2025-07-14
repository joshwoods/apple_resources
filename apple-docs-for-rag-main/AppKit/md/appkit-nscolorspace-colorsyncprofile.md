

- AppKit
- NSColorSpace
-  colorSyncProfile 

Instance Property

# colorSyncProfile

The ColorSync profile from which the color space was created.

macOS

``` source
var colorSyncProfile: UnsafeMutableRawPointer? { get }
```

## Discussion

The ColorSync profile on which the receiver is based. You need to cast this value to an object of opaque type CMProfileRef. Returns `NULL` if the receiver was created from a ICC-profile data instead. See ColorSync Manager for further information on CMProfileRef.

## See Also

### Accessing Color Space Data and Attributes

var cgColorSpace: CGColorSpace?

The Core Graphics color-space object that represents a color space equivalent to the color space’s.

var colorSpaceModel: NSColorSpace.Model

The model on which the color space is based.

enum Model

Constants that describe the abstract model on which color space objects are based.

var iccProfileData: Data?

The ICC profile data from which the color space was created.

var localizedName: String?

The localized name of the color space.

var numberOfColorComponents: Int

The number of components, excluding alpha, the color space supports.

