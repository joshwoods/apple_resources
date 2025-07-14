

- Core Image
- CIDetector
- Detector Configuration Keys
-  CIDetectorNumberOfAngles 

Global Variable

# CIDetectorNumberOfAngles

The number of perspectives to use for detecting a face in video input.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
let CIDetectorNumberOfAngles: String
```

## Discussion

The value for this key is an `NSNumber` object containing the number 1, 3, 5, 7, 9, or 11. At higher numbers of angles, face detection in video becomes more accurate, but at a higher computational cost.

