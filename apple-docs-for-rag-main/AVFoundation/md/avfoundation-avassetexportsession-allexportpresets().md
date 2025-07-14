

- AVFoundation
- AVAssetExportSession
-  allExportPresets() 

Type Method

# allExportPresets()

Returns all available export preset names.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class func allExportPresets() -> [String]
```

## Return Value

See Export Presets for values an asset export session supports.

## Discussion

Not all presets are compatible with all assets.

## See Also

### Accessing Export Presets

var presetName: String

The name of the preset that the asset export session uses.

func determineCompatibleFileTypes(completionHandler: ([AVFileType]) -> Void)

Determines the output file types an asset export session supports writing in its current configuration.

class func determineCompatibility(ofExportPreset: String, with: AVAsset, outputFileType: AVFileType?, completionHandler: (Bool) -> Void)

Determines an export preset’s compatibility to export the asset in a container of the output file type.

class func exportPresets(compatibleWith: AVAsset) -> [String]

Returns compatible export presets for the asset.

Deprecated

