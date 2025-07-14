

- Core Graphics
- CGImage
-  copy(colorSpace:) 

Instance Method

# copy(colorSpace:)

Creates a copy of a bitmap image, replacing its colorspace.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func copy(colorSpace space: CGColorSpace) -> CGImage?
```

## Parameters 

`space`  

The destination color space. The number of components in this color space must be the same as the number in the specified image.

## Return Value

A new CGImage that is a copy of the image passed as the `image` parameter but with its color space replaced by that specified by the `colorspace` parameter. Returns `NULL` if `image` is an image mask, or if the number of components of `colorspace` is not the same as the number of components of the colorspace of `image`. In Objective-C, you’re responsible for releasing this object using CGImageRelease.

## See Also

### Copying an Image

func copy() -> CGImage?

Creates a copy of a bitmap image.

