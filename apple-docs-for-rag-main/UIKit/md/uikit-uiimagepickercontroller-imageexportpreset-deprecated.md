

- UIKit
- UIImagePickerController
-  imageExportPreset Deprecated

Instance Property

# imageExportPreset

The preset to use when preparing images for export to your app.

iOS 11.0–18.4DeprecatediPadOS 11.0–18.4DeprecatedMac Catalyst 13.1+visionOS 1.0–2.4Deprecated

``` source
@MainActor
var imageExportPreset: UIImagePickerController.ImageURLExportPreset { get set }
```

Deprecated

Use PHPickerViewController instead.

## Discussion

The default value of this property is UIImagePickerController.ImageURLExportPreset.compatible.

## See Also

### Configuring the export presets

enum ImageURLExportPreset

Constants that indicate how to export images to the client app.

Deprecated

var videoExportPreset: String

The preset to use when preparing video for export to your app.

Deprecated

