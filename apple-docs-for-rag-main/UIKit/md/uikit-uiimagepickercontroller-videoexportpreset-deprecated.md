

- UIKit
- UIImagePickerController
-  videoExportPreset Deprecated

Instance Property

# videoExportPreset

The preset to use when preparing video for export to your app.

iOS 11.0–18.4DeprecatediPadOS 11.0–18.4DeprecatedMac Catalyst 13.1+visionOS 1.0–2.4Deprecated

``` source
@MainActor
var videoExportPreset: String { get set }
```

Deprecated

Use PHPickerViewController with AVAssetExportSession instead.

## Discussion

The value of this key is one of the export presets supported by the AVAssetExportSession class. For a list of possible values, see the export preset constants in AVAssetExportSession.

## See Also

### Configuring the export presets

var imageExportPreset: UIImagePickerController.ImageURLExportPreset

The preset to use when preparing images for export to your app.

Deprecated

enum ImageURLExportPreset

Constants that indicate how to export images to the client app.

Deprecated

