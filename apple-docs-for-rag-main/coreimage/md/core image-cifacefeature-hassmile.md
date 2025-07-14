

- Core Image
- CIFaceFeature
-  hasSmile 

Instance Property

# hasSmile

A Boolean value that indicates whether a smile is detected in the face.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var hasSmile: Bool { get }
```

## Discussion

For smiles to be detected, the key CIDetectorSmile must be present with a value of `true` in the dictionary passed to a detector’s features(in:options:) method.

## See Also

### Identifying Facial Features

var hasLeftEyePosition: Bool

A Boolean value that indicates whether the detector found the face’s left eye.

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

var leftEyeClosed: Bool

A Boolean value that indicates whether a closed left eye is detected in the face.

var rightEyeClosed: Bool

A Boolean value that indicates whether a closed right eye is detected in the face.

