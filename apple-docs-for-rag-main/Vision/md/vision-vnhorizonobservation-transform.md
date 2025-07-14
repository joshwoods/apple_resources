

- Vision
- VNHorizonObservation
-  transform 

Instance Property

# transform

The transform to apply to the detected horizon.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var transform: CGAffineTransform { get }
```

## Discussion

Apply the transform’s inverse to orient the image in an upright position and make the detected horizon level.

## See Also

### Evaluating the Horizon

var angle: CGFloat

The angle of the observed horizon.

func transform(forImageWidth: Int, height: Int) -> CGAffineTransform

Creates an affine transform for the specified image width and height.

