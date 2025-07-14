

- Core Image
- CIDetector
-  Detector Types 

API Collection

# Detector Types

Strings used to declare the detector for which you are interested.

## Topics

### Constants

let CIDetectorTypeFace: String

A detector that searches for faces in a still image or video, returning CIFaceFeature objects that provide information about detected faces.

let CIDetectorTypeRectangle: String

A detector that searches for rectangular areas in a still image or video, returning CIRectangleFeature objects that provide information about detected regions.

let CIDetectorTypeQRCode: String

A detector that searches for Quick Response codes (a type of 2D barcode) in a still image or video, returning CIQRCodeFeature objects that provide information about detected barcodes.

let CIDetectorTypeText: String

A detector that searches for text in a still image or video, returning CITextFeature objects that provide information about detected regions.

