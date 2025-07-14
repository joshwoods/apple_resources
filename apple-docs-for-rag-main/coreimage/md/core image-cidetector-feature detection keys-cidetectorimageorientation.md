

- Core Image
- CIDetector
- Feature Detection Keys
-  CIDetectorImageOrientation 

Global Variable

# CIDetectorImageOrientation

An option for the display orientation of the image whose features you want to detect.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
let CIDetectorImageOrientation: String
```

## Discussion

The value of this key is an `NSNumber` object whose value is an integer between `1` and `8`. The TIFF and EXIF specifications define these values to indicate where the pixel coordinate origin (0,0) of the image should appear when it is displayed. The default value is `1`, indicating that the origin is in the top left corner of the image. For further details, see kCGImagePropertyOrientation.

Core Image detects only faces whose orientation matches that of the image. You should provide a value for this key if you want to detect faces in a different orientation.

