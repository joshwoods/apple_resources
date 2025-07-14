

- AppKit
- NSImage
-  layerContents(forContentsScale:) 

Instance Method

# layerContents(forContentsScale:)

Returns an object that may be used as the contents of a layer.

macOS 10.7+

``` source
func layerContents(forContentsScale layerContentsScale: CGFloat) -> Any
```

## Parameters 

`layerContentsScale`  

The scale factor for the resulting image. Obtain the value for this parameter by calling the recommendedLayerContentsScale(_:) method.

## Return Value

A object that you can assign to the contents property of a CALayer object. This object contains the image data from the current image optimized for the specified scale factor.

## Discussion

Use this method in situations where you want to use the image as the contents of a layer. This method provides the image data wrapped in an object that correctly respects all of the possible content gravities supported by the layer. Use of the returned object as the layer’s contents is recommended over the use of the `NSImage` object itself.

## See Also

### Using Images with Core Animation

func recommendedLayerContentsScale(CGFloat) -> CGFloat

Returns the recommended layer contents scale for this image.

