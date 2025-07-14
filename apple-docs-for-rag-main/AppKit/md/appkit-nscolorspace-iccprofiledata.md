

- AppKit
- NSColorSpace
-  iccProfileData 

Instance Property

# iccProfileData

The ICC profile data from which the color space was created.

macOS

``` source
var iccProfileData: Data? { get }
```

## Discussion

The ICC profile from which the receiver was created. This method attempts to compute the profile data from a CMProfileRef object and returns `nil` if it is unable to.

For information on ICC profiles, see the latest ICC specification at the International Color Consortium website.

## See Also

### Accessing Color Space Data and Attributes

var cgColorSpace: CGColorSpace?

The Core Graphics color-space object that represents a color space equivalent to the color space’s.

var colorSpaceModel: NSColorSpace.Model

The model on which the color space is based.

enum Model

Constants that describe the abstract model on which color space objects are based.

var colorSyncProfile: UnsafeMutableRawPointer?

The ColorSync profile from which the color space was created.

var localizedName: String?

The localized name of the color space.

var numberOfColorComponents: Int

The number of components, excluding alpha, the color space supports.

