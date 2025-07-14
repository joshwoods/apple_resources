

- AVFoundation
- AVAssetExportSession
-  exportPresets(compatibleWith:) Deprecated

Type Method

# exportPresets(compatibleWith:)

Returns compatible export presets for the asset.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0Deprecated

``` source
class func exportPresets(compatibleWith asset: AVAsset) -> [String]
```

Deprecated

Use determineCompatibility(ofExportPreset:with:outputFileType:completionHandler:) instead.

## Parameters 

`asset`  

An asset to export.

## Return Value

An array of compatible presets. See Export Presets for preset values an asset export session supports.

## Discussion

Not all export presets are compatible with all assets. For example, video-only assets aren’t compatible with an audio-only preset. Call this method to determine the compatible presets for the asset you’re exporting.

Important

Load the asset’s tracks property before calling this method to avoid blocking the calling thread.

## See Also

### Accessing Export Presets

var presetName: String

The name of the preset that the asset export session uses.

func determineCompatibleFileTypes(completionHandler: ([AVFileType]) -> Void)

Determines the output file types an asset export session supports writing in its current configuration.

class func allExportPresets() -> [String]

Returns all available export preset names.

class func determineCompatibility(ofExportPreset: String, with: AVAsset, outputFileType: AVFileType?, completionHandler: (Bool) -> Void)

Determines an export preset’s compatibility to export the asset in a container of the output file type.

