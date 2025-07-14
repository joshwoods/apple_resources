

- Core Image
- CIDetector
- Detector Types
-  CIDetectorTypeFace 

Global Variable

# CIDetectorTypeFace

A detector that searches for faces in a still image or video, returning CIFaceFeature objects that provide information about detected faces.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
let CIDetectorTypeFace: String
```

## Discussion

For better accuracy and performance in face detection, use the CIDetectorImageOrientation key to specify the image orientation when using the features(in:options:) method.

