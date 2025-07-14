

- Core Image
- CIImage
-  oriented(\_:) 

Instance Method

# oriented(\_:)

Transforms the original image by a given CGImagePropertyOrientation and returns the result.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func oriented(_ orientation: CGImagePropertyOrientation) -> CIImage
```

## Discussion

Returns a new image representing the original image transformed for the given CGImagePropertyOrientation.

## See Also

### Working with Orientation

func orientationTransform(for: CGImagePropertyOrientation) -> CGAffineTransform

The affine transform for changing the image to the given orientation.

