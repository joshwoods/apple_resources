

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.AutoFocusRangeRestriction
-  AVCaptureDevice.AutoFocusRangeRestriction.none 

Case

# AVCaptureDevice.AutoFocusRangeRestriction.none

The device attempts to focus on objects at any range.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
case none
```

## Discussion

This value is the default, and the only value allowed on devices that do not support focus range restriction.

## See Also

### Constants

case near

The device primarily attempts to focus on subjects near the camera.

case far

The device primarily attempts to focus on subjects far away from the camera.

