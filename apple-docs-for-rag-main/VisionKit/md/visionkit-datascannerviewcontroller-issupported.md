

- VisionKit
- DataScannerViewController
-  isSupported 

Type Property

# isSupported

A Boolean value that indicates whether the device supports data scanning.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
class var isSupported: Bool { get }
```

## Mentioned in 

Scanning data with the camera

## Discussion

For this property to be `true`, the device must have the A12 Bionic chip or later. This property is `false` for apps running in visionOS.

Important

If your app requires data scanning for its core functionality, you can make your app available only on devices that support data scanning. Add the UIRequiredDeviceCapabilities key to your app’s information property list and include the `iphone-ipad-minimum-performance-a12` subkey in the array of device capabilities.

## See Also

### Handling availability

class var isAvailable: Bool

A Boolean value that indicates whether a person grants your app access to the camera and doesn’t have any restrictions to using the camera.

class var supportedTextRecognitionLanguages: [String]

The identifiers for the languages that the data scanner recognizes.

enum ScanningUnavailable

The possible reasons the data scanner is unavailable.

