

- AppKit
- NSColorSpace
-  colorSpaceModel 

Instance Property

# colorSpaceModel

The model on which the color space is based.

macOS

``` source
var colorSpaceModel: NSColorSpace.Model { get }
```

## Discussion

See `Color Space Models` for a list of valid NSColorSpaceModel constants.

## See Also

### Accessing Color Space Data and Attributes

var cgColorSpace: CGColorSpace?

The Core Graphics color-space object that represents a color space equivalent to the color space’s.

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

