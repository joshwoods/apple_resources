

- Core Image
- CIImageAccumulator
-  setImage(\_:dirtyRect:) 

Instance Method

# setImage(\_:dirtyRect:)

Updates an image accumulator with a subregion of an image object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func setImage(
    _ image: CIImage,
    dirtyRect: CGRect
)
```

## Parameters 

`im`  

The image object whose contents you want to assign to the image accumulator.

`r`  

A rectangle that defines the subregion of the image object that’s changed since the last time you updated the image accumulator. You must guarantee that the new contents differ from the old only within the region specified by the this argument.

## Discussion

For additional details on using this method, see “Imaging Dynamical Systems” in Core Image Programming Guide.

## See Also

### Setting an Image

func setImage(CIImage)

Sets the contents of the image accumulator to the contents of the specified image object.

