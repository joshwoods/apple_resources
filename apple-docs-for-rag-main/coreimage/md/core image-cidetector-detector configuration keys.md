

- Core Image
- CIDetector
-  Detector Configuration Keys 

API Collection

# Detector Configuration Keys

Keys used in the options dictionary to configure a detector.

## Topics

### Constants

let CIDetectorAccuracy: String

A key used to specify the desired accuracy for the detector.

let CIDetectorTracking: String

A key used to enable or disable face tracking for the detector. Use this option when you want to track faces across frames in a video.

let CIDetectorMinFeatureSize: String

A key used to specify the minimum size that the detector will recognize as a feature.

let CIDetectorNumberOfAngles: String

The number of perspectives to use for detecting a face in video input.

let CIDetectorMaxFeatureCount: String

The key to the configuration dictionary whose value represents the maximum number of features the detector should return.

