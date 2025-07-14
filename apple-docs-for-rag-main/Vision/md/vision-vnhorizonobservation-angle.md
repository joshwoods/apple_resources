

- Vision
- VNHorizonObservation
-  angle 

Instance Property

# angle

The angle of the observed horizon.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var angle: CGFloat { get }
```

## Discussion

Use the angle to orient the image in an upright position and make the detected horizon level.

## See Also

### Evaluating the Horizon

var transform: CGAffineTransform

The transform to apply to the detected horizon.

func transform(forImageWidth: Int, height: Int) -> CGAffineTransform

Creates an affine transform for the specified image width and height.

