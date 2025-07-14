

- VisionKit
- DataScannerViewController
-  supportedTextRecognitionLanguages 

Type Property

# supportedTextRecognitionLanguages

The identifiers for the languages that the data scanner recognizes.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
class var supportedTextRecognitionLanguages: [String] { get }
```

## Mentioned in 

Scanning data with the camera

## See Also

### Handling availability

class var isSupported: Bool

A Boolean value that indicates whether the device supports data scanning.

class var isAvailable: Bool

A Boolean value that indicates whether a person grants your app access to the camera and doesn’t have any restrictions to using the camera.

enum ScanningUnavailable

The possible reasons the data scanner is unavailable.

