

- Vision
- VNFaceLandmarks2D
-  leftPupil 

Instance Property

# leftPupil

The region containing the point where the left pupil is located.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var leftPupil: VNFaceLandmarkRegion2D? { get }
```

## Discussion

This value may be inaccurate if the eye is blinking.

## See Also

### Face Landmark Points

var allPoints: VNFaceLandmarkRegion2D?

The region containing all face landmark points.

var faceContour: VNFaceLandmarkRegion2D?

The region containing points that trace the face contour from the left cheek, over the chin, to the right cheek.

var leftEye: VNFaceLandmarkRegion2D?

The region containing points that outline the left eye.

var rightEye: VNFaceLandmarkRegion2D?

The region containing points that outline the right eye.

var leftEyebrow: VNFaceLandmarkRegion2D?

The region containing points that trace the left eyebrow.

var rightEyebrow: VNFaceLandmarkRegion2D?

The region containing points that trace the right eyebrow.

var nose: VNFaceLandmarkRegion2D?

The region containing points that outline the nose.

var noseCrest: VNFaceLandmarkRegion2D?

The region containing points that trace the center crest of the nose.

var medianLine: VNFaceLandmarkRegion2D?

The region containing points that trace a vertical line down the center of the face.

var outerLips: VNFaceLandmarkRegion2D?

The region containing points that outline the outside of the lips.

var innerLips: VNFaceLandmarkRegion2D?

The region containing points that outline the space between the lips.

var rightPupil: VNFaceLandmarkRegion2D?

The region containing the point where the right pupil is located.

