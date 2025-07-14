

- AppKit
- NSColorSpace
-  init(cgColorSpace:) 

Initializer

# init(cgColorSpace:)

Initializes and returns a color space object initialized from a Core Graphics color-space object.

macOS 10.5+

``` source
init?(cgColorSpace: CGColorSpace)
```

## Parameters 

`cgColorSpace`  

A reference to a Core Graphics color-space object (CGColorSpace).

## Return Value

The initialized `NSColorSpace` object or `nil` if initialization was not successful, which might happen if the color space represented by the `CGColorSpace` object is not supported by `NSColorSpace`.

## Discussion

Because `NSColorSpace` might retain or copy the `CGColorSpace` object depending on circumstances, you should not assume pointer equality of the provided object with that returned by cgColorSpace. And even if the pointer equality is preserved during runtime, it may not be after the `NSColorSpace` object is archived and unarchived.

## See Also

### Initializing a Custom Color Space Object

init?(colorSyncProfile: UnsafeMutableRawPointer)

Initializes and returns a color space object from the specified ColorSync profile.

init?(iccProfileData: Data)

Initializes and returns a color space object from the specified ICC profile.

