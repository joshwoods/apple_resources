

- Core Image
- CIFaceFeature
-  faceAngle 

Instance Property

# faceAngle

The rotation of the face.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var faceAngle: Float { get }
```

## Discussion

Rotation is measured counterclockwise in degrees, with zero indicating that a line drawn between the eyes is horizontal relative to the image orientation.

## See Also

### Locating Faces

var bounds: CGRect

A rectangle indicating the position and dimensions of the face in image coordinates.

var hasFaceAngle: Bool

A Boolean value that indicates whether information about face rotation is available.

