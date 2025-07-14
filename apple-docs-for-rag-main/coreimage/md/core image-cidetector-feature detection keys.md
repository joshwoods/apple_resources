

- Core Image
- CIDetector
-  Feature Detection Keys 

API Collection

# Feature Detection Keys

Keys used in the options dictionary for features(in:options:).

## Topics

### Constants

let CIDetectorImageOrientation: String

An option for the display orientation of the image whose features you want to detect.

let CIDetectorEyeBlink: String

An option for whether Core Image will perform additional processing to recognize closed eyes in detected faces.

let CIDetectorSmile: String

An option for whether Core Image will perform additional processing to recognize smiles in detected faces.

let CIDetectorFocalLength: String

An option identifying the focal length in pixels used in capturing images to be processed by the detector.

let CIDetectorAspectRatio: String

An option specifying the aspect ratio (width divided by height) of rectangles to search for.

let CIDetectorReturnSubFeatures: String

An option specifying whether to return feature information for components of detected features.

