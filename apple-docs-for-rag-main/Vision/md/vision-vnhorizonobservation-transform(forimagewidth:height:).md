

- Vision
- VNHorizonObservation
-  transform(forImageWidth:height:) 

Instance Method

# transform(forImageWidth:height:)

Creates an affine transform for the specified image width and height.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func transform(
    forImageWidth width: Int,
    height: Int
) -> CGAffineTransform
```

## Parameters 

`width`  

The width of the image.

`height`  

The height of the image.

## Return Value

An affine transform.

## See Also

### Evaluating the Horizon

var angle: CGFloat

The angle of the observed horizon.

var transform: CGAffineTransform

The transform to apply to the detected horizon.

