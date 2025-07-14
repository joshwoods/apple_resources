

- Core Image
- CIImage
-  orientationTransform(for:) 

Instance Method

# orientationTransform(for:)

The affine transform for changing the image to the given orientation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func orientationTransform(for orientation: CGImagePropertyOrientation) -> CGAffineTransform
```

## Discussion

Returns a CGAffineTransform for the CGImagePropertyOrientation value to apply to the image.

## See Also

### Working with Orientation

func oriented(CGImagePropertyOrientation) -> CIImage

Transforms the original image by a given CGImagePropertyOrientation and returns the result.

