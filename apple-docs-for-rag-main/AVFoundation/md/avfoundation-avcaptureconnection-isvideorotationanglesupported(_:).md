

- AVFoundation
- AVCaptureConnection
-  isVideoRotationAngleSupported(\_:) 

Instance Method

# isVideoRotationAngleSupported(\_:)

Returns a Boolean value that indicates whether the connection supports a rotation angle.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
func isVideoRotationAngleSupported(_ videoRotationAngle: CGFloat) -> Bool
```

## Parameters 

`videoRotationAngle`  

A rotation angle in degrees.

## See Also

### Rotating a video

var videoRotationAngle: CGFloat

A rotation angle the connection applies to a video flowing through it.

