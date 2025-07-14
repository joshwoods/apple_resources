

- AppKit
- NSColorSpace
-  init(colorSyncProfile:) 

Initializer

# init(colorSyncProfile:)

Initializes and returns a color space object from the specified ColorSync profile.

macOS

``` source
init?(colorSyncProfile prof: UnsafeMutableRawPointer)
```

## Parameters 

`prof`  

The ColorSync profile to use when initializing the `NSColorSpace` object. This should be an object of opaque type CMProfileRef. See ColorSync Manager for further information on CMProfileRef.

## Return Value

The initialized `NSColorSpace` object or `nil` if initialization was not successful.

## See Also

### Related Documentation

var colorSyncProfile: UnsafeMutableRawPointer?

The ColorSync profile from which the color space was created.

### Initializing a Custom Color Space Object

init?(cgColorSpace: CGColorSpace)

Initializes and returns a color space object initialized from a Core Graphics color-space object.

init?(iccProfileData: Data)

Initializes and returns a color space object from the specified ICC profile.

