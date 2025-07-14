

- Core Image
- CIBlendKernel
-  apply(foreground:background:) 

Instance Method

# apply(foreground:background:)

Creates a new image using the blend kernel and specified foreground and background images.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func apply(
    foreground: CIImage,
    background: CIImage
) -> CIImage?
```

## Parameters 

`foreground`  

The first input image to be blended

`background`  

The second input image to be blended

## Return Value

A CIImage blending the foreground and background images. Its extent will be the union of the foreground and background image extents.

## Discussion

The foreground and background images are not treated differently in the blending. You can think of them as equivalents A and B; the foreground is not given any precedence over the background.

