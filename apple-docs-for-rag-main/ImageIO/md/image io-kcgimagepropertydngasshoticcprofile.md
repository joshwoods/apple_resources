

- Image I/O
-  kCGImagePropertyDNGAsShotICCProfile 

Global Variable

# kCGImagePropertyDNGAsShotICCProfile

A profile that specifies default color rendering from camera color-space coordinates into the ICC profile space.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
let kCGImagePropertyDNGAsShotICCProfile: CFString
```

## See Also

### Color Calibration

let kCGImagePropertyDNGBlackLevelRepeatDim: CFString

The repeat pattern size for the black level tag.

let kCGImagePropertyDNGBlackLevel: CFString

The zero light encoding level, specified as a repeating pattern.

let kCGImagePropertyDNGBlackLevelDeltaH: CFString

The difference between the zero-light encoding level for each column and the baseline zero-light encoding level.

let kCGImagePropertyDNGBlackLevelDeltaV: CFString

The difference between the zero-light encodoing level for each row and the baseline zero-light encoding level.

let kCGImagePropertyDNGWhiteLevel: CFString

The saturated encoding level for the raw sample values.

let kCGImagePropertyDNGCalibrationIlluminant1: CFString

The illuminant for the first set of color calibration tags.

let kCGImagePropertyDNGCalibrationIlluminant2: CFString

The illuminant for an optional second set of color calibration tags.

let kCGImagePropertyDNGColorMatrix1: CFString

A transformation matrix that converts XYZ values to reference camera native color spaces, under the first calibration illuminant.

let kCGImagePropertyDNGColorMatrix2: CFString

A transformation matrix that converts XYZ values to reference camera native color spaces, under the second calibration illuminant.

let kCGImagePropertyDNGCameraCalibration1: CFString

A matrix that transforms reference camera native space values to camera-native space values under the first calibration illuminant.

let kCGImagePropertyDNGCameraCalibration2: CFString

A matrix that transforms reference camera native space values to camera-native space values under the second calibration illuminant.

let kCGImagePropertyDNGReductionMatrix1: CFString

A reduction matrix that converts color camera-native space values to XYZ values, under the first calibration illuminant.

let kCGImagePropertyDNGReductionMatrix2: CFString

A reduction matrix that converts color camera-native space values to XYZ values, under the second calibration illuminant.

let kCGImagePropertyDNGAsShotPreProfileMatrix: CFString

A matrix to apply to the camera color-space coordinates before processing values through the ICC profile.

let kCGImagePropertyDNGCurrentICCProfile: CFString

A profile that specifies default color rendering from camera color-space coordinates into the ICC profile space.

