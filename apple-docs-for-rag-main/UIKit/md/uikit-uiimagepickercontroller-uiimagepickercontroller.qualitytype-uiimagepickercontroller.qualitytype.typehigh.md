

- UIKit
- UIImagePickerController
- UIImagePickerController.QualityType
-  UIImagePickerController.QualityType.typeHigh 

Case

# UIImagePickerController.QualityType.typeHigh

If recording, specifies that you want to use the highest-quality video recording supported for the active camera on the device.

iOSiPadOSMac Catalyst

``` source
case typeHigh
```

## Discussion

Recorded files are suitable for on-device playback and for wired transfer to the Desktop using Image Capture; they are likely to be too large for transfer using Wi-Fi.

If displaying a recorded movie in the image picker, specifies that you do not want to reduce the video quality of the movie.

## See Also

### Constants

case type640x480

If recording, specifies that you want to use VGA-quality video recording (pixel dimensions of 640x480).

case typeMedium

If recording, specifies that you want to use medium-quality video recording.

case typeLow

If recording, specifies that you want to use low-quality video recording.

case typeIFrame1280x720

If recording, specifies that you want to use 1280x720 iFrame format.

case typeIFrame960x540

If recording, specifies that you want to use 960x540 iFrame format.

