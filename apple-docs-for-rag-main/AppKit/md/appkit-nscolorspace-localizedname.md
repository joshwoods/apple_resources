

- AppKit
- NSColorSpace
-  localizedName 

Instance Property

# localizedName

The localized name of the color space.

macOS

``` source
var localizedName: String? { get }
```

## Discussion

This property holds the name of the color space as a localized string or `nil` if no localized name exists.

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

var iccProfileData: Data?

The ICC profile data from which the color space was created.

var numberOfColorComponents: Int

The number of components, excluding alpha, the color space supports.

