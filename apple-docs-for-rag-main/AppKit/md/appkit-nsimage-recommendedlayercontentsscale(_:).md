

- AppKit
- NSImage
-  recommendedLayerContentsScale(\_:) 

Instance Method

# recommendedLayerContentsScale(\_:)

Returns the recommended layer contents scale for this image.

macOS 10.7+

``` source
func recommendedLayerContentsScale(_ preferredContentsScale: CGFloat) -> CGFloat
```

## Parameters 

`preferredContentsScale`  

The preferred layer contents scale. Don’t use a higher scale factor if the image can’t provide it. If the image is resolution independent the return value will be the same as the input. If you specify `0.0` for this parameter, the method uses the scale factor for the default screen.

## Return Value

The recommended layer contents scale. This scale factor may be different than the one in the `preferredContentsScale` parameter.

## Discussion

Use this method to obtain the scale factor value that you pass to the layerContents(forContentsScale:) method. This method uses the image data to determine the scale factor that is best suited for creating an image that looks good in the layer.

## See Also

### Using Images with Core Animation

func layerContents(forContentsScale: CGFloat) -> Any

Returns an object that may be used as the contents of a layer.

