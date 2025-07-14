

- Core Image
- CIFaceFeature
-  hasLeftEyePosition 

Instance Property

# hasLeftEyePosition

A Boolean value that indicates whether the detector found the face’s left eye.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var hasLeftEyePosition: Bool { get }
```

## See Also

### Identifying Facial Features

var hasRightEyePosition: Bool

A Boolean value that indicates whether the detector found the face’s right eye.

var hasMouthPosition: Bool

A Boolean value that indicates whether the detector found the face’s mouth.

var leftEyePosition: CGPoint

The coordinates of the left eye, in image coordinates.

var rightEyePosition: CGPoint

The coordinates of the right eye, in image coordinates

var mouthPosition: CGPoint

The coordinates of the mouth, in image coordinates

var hasSmile: Bool

A Boolean value that indicates whether a smile is detected in the face.

var leftEyeClosed: Bool

A Boolean value that indicates whether a closed left eye is detected in the face.

var rightEyeClosed: Bool

A Boolean value that indicates whether a closed right eye is detected in the face.

