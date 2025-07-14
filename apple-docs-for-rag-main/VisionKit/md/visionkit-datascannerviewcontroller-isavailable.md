

- VisionKit
- DataScannerViewController
-  isAvailable 

Type Property

# isAvailable

A Boolean value that indicates whether a person grants your app access to the camera and doesn’t have any restrictions to using the camera.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
class var isAvailable: Bool { get }
```

## Mentioned in 

Scanning data with the camera

## Discussion

For example, this property may be `false` if a person has Screen Time restrictions.

## See Also

### Handling availability

class var isSupported: Bool

A Boolean value that indicates whether the device supports data scanning.

class var supportedTextRecognitionLanguages: [String]

The identifiers for the languages that the data scanner recognizes.

enum ScanningUnavailable

The possible reasons the data scanner is unavailable.

