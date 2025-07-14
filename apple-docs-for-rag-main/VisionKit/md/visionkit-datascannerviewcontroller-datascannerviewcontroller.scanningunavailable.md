

- VisionKit
- DataScannerViewController
-  DataScannerViewController.ScanningUnavailable 

Enumeration

# DataScannerViewController.ScanningUnavailable

The possible reasons the data scanner is unavailable.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
enum ScanningUnavailable
```

## Topics

### Unavailable errors

case unsupported

The data scanner isn’t supported on this device.

case cameraRestricted

The data scanner isn’t available due to user restrictions on the use of the camera.

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Related Documentation

func dataScanner(DataScannerViewController, becameUnavailableWithError: DataScannerViewController.ScanningUnavailable)

Responds when the data scanner becomes unavailable and stops scanning.

**Required** Default implementation provided.

### Handling availability

class var isSupported: Bool

A Boolean value that indicates whether the device supports data scanning.

class var isAvailable: Bool

A Boolean value that indicates whether a person grants your app access to the camera and doesn’t have any restrictions to using the camera.

class var supportedTextRecognitionLanguages: [String]

The identifiers for the languages that the data scanner recognizes.

