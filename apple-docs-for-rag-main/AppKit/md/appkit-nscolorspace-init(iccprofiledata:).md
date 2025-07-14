

- AppKit
- NSColorSpace
-  init(iccProfileData:) 

Initializer

# init(iccProfileData:)

Initializes and returns a color space object from the specified ICC profile.

macOS

``` source
init?(iccProfileData iccData: Data)
```

## Parameters 

`iccData`  

The ICC profile to use when initializing the `NSColorSpace` object. For information on ICC profiles, see the latest ICC specification at the International Color Consortium website website.

## Return Value

The initialized `NSColorSpace` object or `nil` if initialization was not successful.

## See Also

### Related Documentation

var iccProfileData: Data?

The ICC profile data from which the color space was created.

### Initializing a Custom Color Space Object

init?(cgColorSpace: CGColorSpace)

Initializes and returns a color space object initialized from a Core Graphics color-space object.

init?(colorSyncProfile: UnsafeMutableRawPointer)

Initializes and returns a color space object from the specified ColorSync profile.

