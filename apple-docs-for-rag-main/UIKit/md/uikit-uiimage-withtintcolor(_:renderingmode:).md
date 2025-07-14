

- UIKit
- UIImage
-  withTintColor(\_:renderingMode:) 

Instance Method

# withTintColor(\_:renderingMode:)

Returns a new version of the image with a tint color that uses the specified rendering mode.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func withTintColor(
    _ color: UIColor,
    renderingMode: UIImage.RenderingMode
) -> UIImage
```

## Parameters 

`color`  

The tint color to apply to the image.

`renderingMode`  

The rendering mode to assign to the returned image.

## Return Value

A new version of the image that incorporates the specified tint color.

## Discussion

For bitmap images, this method draws the background tint color followed by the image contents using the CGBlendMode.destinationIn mode. For symbol images, this method returns an image that always uses the specified tint color.

## See Also

### Tinting the image

func withTintColor(UIColor) -> UIImage

Returns a new version of the current image with the specified tint color.

