

- Vision
- VNImageBasedRequest
-  regionOfInterest 

Instance Property

# regionOfInterest

The region of the image in which Vision will perform the request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var regionOfInterest: CGRect { get set }
```

## Mentioned in 

Detecting Human Body Poses in Images

## Discussion

The rectangle is normalized to the dimensions of the processed image. Its origin is specified relative to the image’s lower-left corner.

The default value is `{ { 0, 0 }, { 1, 1 } }`.

Important

The request will fail to perform if you set this property to a rectangle outside the normalized coordinate space.

