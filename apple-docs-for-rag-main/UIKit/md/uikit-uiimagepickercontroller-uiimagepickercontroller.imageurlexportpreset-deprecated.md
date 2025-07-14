

- UIKit
- UIImagePickerController
-  UIImagePickerController.ImageURLExportPreset Deprecated

Enumeration

# UIImagePickerController.ImageURLExportPreset

Constants that indicate how to export images to the client app.

iOS 11.0–18.4DeprecatediPadOS 11.0–18.4DeprecatedMac Catalyst 13.1+visionOS 1.0–2.4Deprecated

``` source
enum ImageURLExportPreset
```

Deprecated

Use PHPickerViewController instead.

## Topics

### Constants

case compatible

A preset for converting HEIF formatted images to JPEG.

case current

A preset for passing image data as-is to the client.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the export presets

var imageExportPreset: UIImagePickerController.ImageURLExportPreset

The preset to use when preparing images for export to your app.

Deprecated

var videoExportPreset: String

The preset to use when preparing video for export to your app.

Deprecated

