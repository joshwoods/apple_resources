

- Vision
- HorizonObservation
-  transform 

Instance Property

# transform

The transform to apply to the detected horizon.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let transform: CGAffineTransform
```

## Discussion

Apply the transform’s inverse to orient the image in an upright position and make the detected horizon level.

## See Also

### Getting the transform

func transform(for: CGSize) -> CGAffineTransform

Creates an affine transform for the specified image width and height.

