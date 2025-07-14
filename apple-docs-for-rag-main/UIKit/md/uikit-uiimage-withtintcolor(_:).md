

- UIKit
- UIImage
-  withTintColor(\_:) 

Instance Method

# withTintColor(\_:)

Returns a new version of the current image with the specified tint color.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func withTintColor(_ color: UIColor) -> UIImage
```

## Parameters 

`color`  

The tint color to apply to the image.

## Return Value

A new version of the image that incorporates the specified tint color.

## Discussion

For bitmap images, this method draws the background tint color followed by the image contents using the CGBlendMode.destinationIn mode. For symbol images, this method returns an image that always uses the specified tint color.

The new image uses the same rendering mode as the original image.

## See Also

### Tinting the image

func withTintColor(UIColor, renderingMode: UIImage.RenderingMode) -> UIImage

Returns a new version of the image with a tint color that uses the specified rendering mode.

