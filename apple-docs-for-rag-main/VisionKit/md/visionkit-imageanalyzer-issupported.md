

- VisionKit
- ImageAnalyzer
-  isSupported 

Type Property

# isSupported

A Boolean value that indicates whether the device supports image analysis.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
final class var isSupported: Bool { get }
```

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

Check this property at runtime to determine if the device supports finding text, machine-readable codes, and subjects in images. The system sets this property to `true` on devices that have an A12 Bionic chip or later.

For more information on the kinds of things the analyzer finds in images, see ImageAnalyzer.AnalysisTypes.

Note

If image analysis is a fundamental requirement for your app’s operation, you can prevent unsupported devices from installing your app. Add the UIRequiredDeviceCapabilities key to your app’s `Info.plist` (or update the key if it’s already present) and include the array member `iphone-ipad-minimum-performance-a12`.

## See Also

### Handling availability

class var supportedTextRecognitionLanguages: [String]

The identifiers for the languages that the image analyzer recognizes.

